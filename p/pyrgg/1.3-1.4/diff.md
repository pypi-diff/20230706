# Comparing `tmp/pyrgg-1.3.tar.gz` & `tmp/pyrgg-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrgg-1.3.tar", last modified: Wed Nov 30 13:23:27 2022, max compression
+gzip compressed data, was "pyrgg-1.4.tar", last modified: Thu Jul  6 18:56:55 2023, max compression
```

## Comparing `pyrgg-1.3.tar` & `pyrgg-1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:23:27.191524 pyrgg-1.3/
--rw-r--r--   0 runner    (1001) docker     (122)      554 2022-11-30 13:23:18.000000 pyrgg-1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (122)     4888 2022-11-30 13:23:18.000000 pyrgg-1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2022-11-30 13:23:18.000000 pyrgg-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      174 2022-11-30 13:23:18.000000 pyrgg-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    26759 2022-11-30 13:23:27.191524 pyrgg-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      777 2022-11-30 13:23:18.000000 pyrgg-1.3/PYRGG.spec
--rw-r--r--   0 runner    (1001) docker     (122)    20030 2022-11-30 13:23:18.000000 pyrgg-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-11-30 13:23:18.000000 pyrgg-1.3/TODO.md
--rw-r--r--   0 runner    (1001) docker     (122)      199 2022-11-30 13:23:18.000000 pyrgg-1.3/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      187 2022-11-30 13:23:18.000000 pyrgg-1.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:23:27.191524 pyrgg-1.3/paper/
--rw-r--r--   0 runner    (1001) docker     (122)   198309 2022-11-30 13:23:18.000000 pyrgg-1.3/paper/10.21105.joss.00331.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      837 2022-11-30 13:23:18.000000 pyrgg-1.3/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2022-11-30 13:23:18.000000 pyrgg-1.3/paper/paper.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:23:27.191524 pyrgg-1.3/pyrgg/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-11-30 13:23:18.000000 pyrgg-1.3/pyrgg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3620 2022-11-30 13:23:18.000000 pyrgg-1.3/pyrgg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18582 2022-11-30 13:23:18.000000 pyrgg-1.3/pyrgg/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    29378 2022-11-30 13:23:18.000000 pyrgg-1.3/pyrgg/graph_gen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3065 2022-11-30 13:23:18.000000 pyrgg-1.3/pyrgg/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    23861 2022-11-30 13:23:18.000000 pyrgg-1.3/pyrgg/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:23:27.191524 pyrgg-1.3/pyrgg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    26759 2022-11-30 13:23:27.000000 pyrgg-1.3/pyrgg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      501 2022-11-30 13:23:27.000000 pyrgg-1.3/pyrgg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 13:23:27.000000 pyrgg-1.3/pyrgg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-30 13:23:27.000000 pyrgg-1.3/pyrgg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-30 13:23:27.000000 pyrgg-1.3/pyrgg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-30 13:23:27.000000 pyrgg-1.3/pyrgg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-30 13:23:18.000000 pyrgg-1.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-11-30 13:23:18.000000 pyrgg-1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-30 13:23:27.191524 pyrgg-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3399 2022-11-30 13:23:18.000000 pyrgg-1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      202 2022-11-30 13:23:18.000000 pyrgg-1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:56:55.319202 pyrgg-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-06 18:56:45.000000 pyrgg-1.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-06 18:56:45.000000 pyrgg-1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-06 18:56:45.000000 pyrgg-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 18:56:45.000000 pyrgg-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26359 2023-07-06 18:56:55.319202 pyrgg-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 18:56:45.000000 pyrgg-1.4/PYRGG.spec
+-rw-r--r--   0 runner    (1001) docker     (123)    19305 2023-07-06 18:56:45.000000 pyrgg-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-06 18:56:45.000000 pyrgg-1.4/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-06 18:56:45.000000 pyrgg-1.4/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 18:56:45.000000 pyrgg-1.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:56:55.315202 pyrgg-1.4/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)   198309 2023-07-06 18:56:45.000000 pyrgg-1.4/paper/10.21105.joss.00331.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-06 18:56:45.000000 pyrgg-1.4/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 18:56:45.000000 pyrgg-1.4/paper/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:56:55.315202 pyrgg-1.4/pyrgg/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 18:56:45.000000 pyrgg-1.4/pyrgg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-06 18:56:45.000000 pyrgg-1.4/pyrgg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-07-06 18:56:45.000000 pyrgg-1.4/pyrgg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29378 2023-07-06 18:56:45.000000 pyrgg-1.4/pyrgg/graph_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-06 18:56:45.000000 pyrgg-1.4/pyrgg/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-06 18:56:45.000000 pyrgg-1.4/pyrgg/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:56:55.319202 pyrgg-1.4/pyrgg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26359 2023-07-06 18:56:55.000000 pyrgg-1.4/pyrgg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-06 18:56:55.000000 pyrgg-1.4/pyrgg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:56:55.000000 pyrgg-1.4/pyrgg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 18:56:55.000000 pyrgg-1.4/pyrgg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 18:56:55.000000 pyrgg-1.4/pyrgg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 18:56:55.000000 pyrgg-1.4/pyrgg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 18:56:45.000000 pyrgg-1.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 18:56:45.000000 pyrgg-1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:56:55.319202 pyrgg-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-06 18:56:45.000000 pyrgg-1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 18:56:45.000000 pyrgg-1.4/tox.ini
```

### Comparing `pyrgg-1.3/AUTHORS.md` & `pyrgg-1.4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/CHANGELOG.md` & `pyrgg-1.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.4] - 2023-07-06
+### Added
+- `check_for_config` function
+- `load_config` function
+- `save_config` function
+### Changed
+- `README.md` modified
+- Logo changed
+- `codecov` removed from `dev-requirements.txt`
+- Test system modified
+- Error messages updated
 ## [1.3] - 2022-11-30
 ### Added
 - Graphviz(DOT) format
 ### Changed
 - [asciinema](https://asciinema.org) instruction video updated
 - Test system modified
 - `README.md` modified
@@ -154,15 +165,16 @@
 
 ## [0.1] - 2017-08-19
 ### Added
 - DIMACS format
 - JSON format
 - README
 
-[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.3...dev
+[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.4...dev
+[1.4]: https://github.com/sepandhaghighi/pyrgg/compare/v1.3...v1.4
 [1.3]: https://github.com/sepandhaghighi/pyrgg/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/pyrgg/compare/v1.1...v1.2
 [1.1]: https://github.com/sepandhaghighi/pyrgg/compare/v1.0...v1.1
 [1.0]: https://github.com/sepandhaghighi/pyrgg/compare/v0.9...v1.0
 [0.9]: https://github.com/sepandhaghighi/pyrgg/compare/v0.8...v0.9
 [0.8]: https://github.com/sepandhaghighi/pyrgg/compare/v0.7...v0.8
 [0.7]: https://github.com/sepandhaghighi/pyrgg/compare/v0.6...v0.7
```

### Comparing `pyrgg-1.3/LICENSE` & `pyrgg-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/PKG-INFO` & `pyrgg-1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrgg
-Version: 1.3
+Version: 1.4
 Summary: Python Random Graph Generator
 Home-page: https://github.com/sepandhaghighi/pyrgg
-Download-URL: https://github.com/sepandhaghighi/pyrgg/tarball/v1.3
+Download-URL: https://github.com/sepandhaghighi/pyrgg/tarball/v1.4
 Author: PyRGG Development Team
 Author-email: info@pyrgg.ir
 License: MIT
 Project-URL: Webpage, https://www.pyrgg.ir
 Project-URL: Source, https://github.com/sepandhaghighi/pyrgg
 Keywords: random graph python3 python generator graph-process generator DIMACS JSON YAML Pickle CSV TSV WEL ASP TGF UCINET
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,44 +36,45 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
-
-							
-
-
 <div align="center">
-<img src="http://www.shaghighi.ir/pyrgg/images/pyrgg-logo.png" height=240px width=320px>
-<hr/>
-<h1>Random Graph Generator</h1>
-
-<a href="http://www.shaghighi.ir/pyrgg"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=website"></a>
-<a href="https://badge.fury.io/py/pyrgg"><img src="https://badge.fury.io/py/pyrgg.svg" alt="PyPI version" height="18"></a>
-<a href="https://anaconda.org/sepandhaghighi/pyrgg"><img src="https://anaconda.org/sepandhaghighi/pyrgg/badges/version.svg"></a>
-<a href="https://codecov.io/gh/sepandhaghighi/pyrgg">
-  <img src="https://codecov.io/gh/sepandhaghighi/pyrgg/branch/master/graph/badge.svg" alt="Codecov" /></a>
-<a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
-<a href="https://discord.gg/dfYAWVMaCW">
-  <img src="https://img.shields.io/discord/1013411447130308669.svg" alt="Discord Channel">
-</a>
+	<img src="https://github.com/sepandhaghighi/pyrgg/raw/master/otherfile/logo.png" width="450">
+	<h1>PyRGG: Python Random Graph Generator</h1>
+	<a href="http://www.shaghighi.ir/pyrgg">
+		<img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=website">
+	</a>
+	<a href="https://badge.fury.io/py/pyrgg">
+		<img src="https://badge.fury.io/py/pyrgg.svg" alt="PyPI version" height="18">
+	</a>
+	<a href="https://anaconda.org/sepandhaghighi/pyrgg">
+		<img src="https://anaconda.org/sepandhaghighi/pyrgg/badges/version.svg">
+	</a>
+	<a href="https://codecov.io/gh/sepandhaghighi/pyrgg">
+  		<img src="https://codecov.io/gh/sepandhaghighi/pyrgg/branch/master/graph/badge.svg" alt="Codecov">
+	</a>
+	<a href="https://www.python.org/">
+		<img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3">
+	</a>
+	<a href="https://discord.gg/dfYAWVMaCW">
+  		<img src="https://img.shields.io/discord/1013411447130308669.svg" alt="Discord Channel">
+	</a>
 </div>	
 
-----------
 ## Table of Contents					
    * [Overview](https://github.com/sepandhaghighi/pyrgg#overview)
    * [Installation](https://github.com/sepandhaghighi/pyrgg#installation)
    * [Usage](https://github.com/sepandhaghighi/pyrgg#usage)
    * [Supported Formats](https://github.com/sepandhaghighi/pyrgg#supported-formats)
    * [Example of Usage](https://github.com/sepandhaghighi/pyrgg#example-of-usage)
    * [Similar Works](https://github.com/sepandhaghighi/pyrgg#similar-works)
    * [Issues & Bug Reports](https://github.com/sepandhaghighi/pyrgg#issues--bug-reports)
-   * [Dependencies](https://github.com/sepandhaghighi/pyrgg#dependencies)
    * [Contribution](https://github.com/sepandhaghighi/pyrgg/blob/master/.github/CONTRIBUTING.md)
    * [References](https://github.com/sepandhaghighi/pyrgg#references)
    * [Citing](https://github.com/sepandhaghighi/pyrgg#citing)
    * [Authors](https://github.com/sepandhaghighi/pyrgg/blob/master/AUTHORS.md)
    * [License](https://github.com/sepandhaghighi/pyrgg/blob/master/LICENSE)
    * [Show Your Support](https://github.com/sepandhaghighi/pyrgg#show-your-support)
    * [Todo](https://github.com/sepandhaghighi/pyrgg/blob/master/TODO.md)
@@ -124,32 +125,31 @@
 		<td align="center"><a href="https://www.codefactor.io/repository/github/sepandhaghighi/pyrgg"><img src="https://www.codefactor.io/repository/github/sepandhaghighi/pyrgg/badge" alt="CodeFactor" /></a></td>	
 	</tr>
 </table>
 
 
 ## Installation		
 
-### Source Code
-- Download [Version 1.3](https://github.com/sepandhaghighi/pyrgg/archive/v1.3.zip) or [Latest Source ](https://github.com/sepandhaghighi/pyrgg/archive/dev.zip)
-- `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
-- `python3 setup.py install` or `python setup.py install` (Need root access)				
-
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install pyrgg==1.3` or `pip3 install pyrgg==1.3` (Need root access)							
+- `pip install pyrgg==1.4` (Need root access)							
+
+### Source Code
+- Download [Version 1.4](https://github.com/sepandhaghighi/pyrgg/archive/v1.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/pyrgg/archive/dev.zip)
+- `pip install .` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io)
 - `conda install -c sepandhaghighi pyrgg` (Need root access)	
 
 ### Exe Version (Only Windows)
-- Download [Exe-Version 1.3](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.3/PYRGG-1.3.exe)
-- Run `PYRGG-1.3.exe`
+- Download [Exe-Version 1.4](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.4/PYRGG-1.4.exe)
+- Run `PYRGG-1.4.exe`
 
 ### System Requirements
 Pyrgg will likely run on a modern dual core PC. Typical configuration is:
 
 - Dual Core CPU (2.0 Ghz+)
 - 4GB of RAM
 
@@ -510,27 +510,14 @@
 
 You can also join our discord server			
 
 <a href="https://discord.gg/dfYAWVMaCW">
   <img src="https://img.shields.io/discord/1013411447130308669.svg?style=for-the-badge" alt="Discord Channel">
 </a>
 
-## Dependencies
-
-<table>
-	<tr> 
-		<td align="center">master</td>	
-		<td align="center">dev</td>	
-	</tr>
-	<tr>
-		<td align="center"><a href="https://requires.io/github/sepandhaghighi/pyrgg/requirements/?branch=master"><img src="https://requires.io/github/sepandhaghighi/pyrgg/requirements.svg?branch=master" alt="Requirements Status" /></a></td>
-		<td align="center"><a href="https://requires.io/github/sepandhaghighi/pyrgg/requirements/?branch=dev"><img src="https://requires.io/github/sepandhaghighi/pyrgg/requirements.svg?branch=dev" alt="Requirements Status" /></a></td>
-	</tr>
-</table>
-
 
 ## Citing
 
 If you use pyrgg in your research, please cite the [JOSS paper](http://joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg JOSS Paper") ;-)
 
 <pre>
 @article{Haghighi2017,
@@ -583,14 +570,17 @@
 <blockquote>10- Skiena, Steven S. The algorithm design manual. Springer International Publishing, 2020. </blockquote>
 
 <blockquote>11- Chakrabarti, Deepayan, Yiping Zhan, and Christos Faloutsos. "R-MAT: A recursive model for graph mining." Proceedings of the 2004 SIAM International Conference on Data Mining. Society for Industrial and Applied Mathematics, 2004. </blockquote>
 
 <blockquote>12- Zhong, Jianlong, and Bingsheng He. "An overview of medusa: simplified graph processing on gpus." ACM SIGPLAN Notices 47.8 (2012): 283-284.</blockquote>
 
 <blockquote>13- Ellson, John, et al. "Graphviz and dynagraph—static and dynamic graph drawing tools." Graph drawing software. Springer, Berlin, Heidelberg, 2004. 127-148.</blockquote>
+
+
+* Logo designed by [Zahra Mobasher](https://www.instagram.com/littleblackoyster)	
 					
  
 ## Show Your Support
 								
 <h3>Star This Repo</h3>					
 
 Give a ⭐️ if this project helped you!
@@ -618,22 +608,35 @@
 <h4>Stellar</h4>		
 GALPOLPISRHIYHLQER2TLJRGUSZH52RYDK6C3HIU4PSMNAV65Q36EGNL
 <h4>Zilliqa</h4>
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 <h4>Coffeete</h4>
 <a href="http://www.coffeete.ir/opensource">
 <img src="http://www.coffeete.ir/images/buttons/lemonchiffon.png" style="width:260px;" />
-</a>	
+</a>
+
+
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.4] - 2023-07-06
+### Added
+- `check_for_config` function
+- `load_config` function
+- `save_config` function
+### Changed
+- `README.md` modified
+- Logo changed
+- `codecov` removed from `dev-requirements.txt`
+- Test system modified
+- Error messages updated
 ## [1.3] - 2022-11-30
 ### Added
 - Graphviz(DOT) format
 ### Changed
 - [asciinema](https://asciinema.org) instruction video updated
 - Test system modified
 - `README.md` modified
@@ -779,15 +782,16 @@
 
 ## [0.1] - 2017-08-19
 ### Added
 - DIMACS format
 - JSON format
 - README
 
-[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.3...dev
+[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.4...dev
+[1.4]: https://github.com/sepandhaghighi/pyrgg/compare/v1.3...v1.4
 [1.3]: https://github.com/sepandhaghighi/pyrgg/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/pyrgg/compare/v1.1...v1.2
 [1.1]: https://github.com/sepandhaghighi/pyrgg/compare/v1.0...v1.1
 [1.0]: https://github.com/sepandhaghighi/pyrgg/compare/v0.9...v1.0
 [0.9]: https://github.com/sepandhaghighi/pyrgg/compare/v0.8...v0.9
 [0.8]: https://github.com/sepandhaghighi/pyrgg/compare/v0.7...v0.8
 [0.7]: https://github.com/sepandhaghighi/pyrgg/compare/v0.6...v0.7
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pyrgg Version: 1.3 Summary: Python Random Graph
+Metadata-Version: 2.1 Name: pyrgg Version: 1.4 Summary: Python Random Graph
 Generator Home-page: https://github.com/sepandhaghighi/pyrgg Download-URL:
-https://github.com/sepandhaghighi/pyrgg/tarball/v1.3 Author: PyRGG Development
+https://github.com/sepandhaghighi/pyrgg/tarball/v1.4 Author: PyRGG Development
 Team Author-email: info@pyrgg.ir License: MIT Project-URL: Webpage, https://
 www.pyrgg.ir Project-URL: Source, https://github.com/sepandhaghighi/pyrgg
 Keywords: random graph python3 python generator graph-process generator DIMACS
 JSON YAML Pickle CSV TSV WEL ASP TGF UCINET Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -19,73 +19,68 @@
 Analysis Classifier: Topic :: Education Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Human Machine
 Interfaces Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.md
-            [http://www.shaghighi.ir/pyrgg/images/pyrgg-logo.png]
-===============================================================================
-                     ****** Random Graph Generator ******
+    [https://github.com/sepandhaghighi/pyrgg/raw/master/otherfile/logo.png]
+              ****** PyRGG: Python Random Graph Generator ******
             [https://img.shields.io/website-up-down-green-red/http/
       shields.io.svg?label=website] [PyPI_version] [https://anaconda.org/
    sepandhaghighi/pyrgg/badges/version.svg] [Codecov] [built_with_Python3]
                                [Discord_Channel]
- ---------- ## Table of Contents * [Overview](https://github.com/
-sepandhaghighi/pyrgg#overview) * [Installation](https://github.com/
-sepandhaghighi/pyrgg#installation) * [Usage](https://github.com/sepandhaghighi/
-pyrgg#usage) * [Supported Formats](https://github.com/sepandhaghighi/
-pyrgg#supported-formats) * [Example of Usage](https://github.com/
-sepandhaghighi/pyrgg#example-of-usage) * [Similar Works](https://github.com/
-sepandhaghighi/pyrgg#similar-works) * [Issues & Bug Reports](https://
-github.com/sepandhaghighi/pyrgg#issues--bug-reports) * [Dependencies](https://
-github.com/sepandhaghighi/pyrgg#dependencies) * [Contribution](https://
-github.com/sepandhaghighi/pyrgg/blob/master/.github/CONTRIBUTING.md) *
-[References](https://github.com/sepandhaghighi/pyrgg#references) * [Citing]
-(https://github.com/sepandhaghighi/pyrgg#citing) * [Authors](https://
-github.com/sepandhaghighi/pyrgg/blob/master/AUTHORS.md) * [License](https://
-github.com/sepandhaghighi/pyrgg/blob/master/LICENSE) * [Show Your Support]
-(https://github.com/sepandhaghighi/pyrgg#show-your-support) * [Todo](https://
-github.com/sepandhaghighi/pyrgg/blob/master/TODO.md) * [Changelog](https://
-github.com/sepandhaghighi/pyrgg/blob/master/CHANGELOG.md) * [Code of Conduct]
-(https://github.com/sepandhaghighi/pyrgg/blob/master/.github/
-CODE_OF_CONDUCT.md) ## Overview Pyrgg is an easy-to-use synthetic random graph
-generator written in Python which supports various graph file formats including
-DIMACS_.gr files. Pyrgg has the ability to generate graphs of different sizes
-and is designed to provide input files for broad range of graph-based research
-applications, including but not limited to testing, benchmarking and
-performance-analysis of graph processing frameworks. Pyrgg target audiences are
-computer scientists who study graph algorithms and graph processing frameworks.
+ ## Table of Contents * [Overview](https://github.com/sepandhaghighi/
+pyrgg#overview) * [Installation](https://github.com/sepandhaghighi/
+pyrgg#installation) * [Usage](https://github.com/sepandhaghighi/pyrgg#usage) *
+[Supported Formats](https://github.com/sepandhaghighi/pyrgg#supported-formats)
+* [Example of Usage](https://github.com/sepandhaghighi/pyrgg#example-of-usage)
+* [Similar Works](https://github.com/sepandhaghighi/pyrgg#similar-works) *
+[Issues & Bug Reports](https://github.com/sepandhaghighi/pyrgg#issues--bug-
+reports) * [Contribution](https://github.com/sepandhaghighi/pyrgg/blob/
+master/.github/CONTRIBUTING.md) * [References](https://github.com/
+sepandhaghighi/pyrgg#references) * [Citing](https://github.com/sepandhaghighi/
+pyrgg#citing) * [Authors](https://github.com/sepandhaghighi/pyrgg/blob/master/
+AUTHORS.md) * [License](https://github.com/sepandhaghighi/pyrgg/blob/master/
+LICENSE) * [Show Your Support](https://github.com/sepandhaghighi/pyrgg#show-
+your-support) * [Todo](https://github.com/sepandhaghighi/pyrgg/blob/master/
+TODO.md) * [Changelog](https://github.com/sepandhaghighi/pyrgg/blob/master/
+CHANGELOG.md) * [Code of Conduct](https://github.com/sepandhaghighi/pyrgg/blob/
+master/.github/CODE_OF_CONDUCT.md) ## Overview Pyrgg is an easy-to-use
+synthetic random graph generator written in Python which supports various graph
+file formats including DIMACS_.gr files. Pyrgg has the ability to generate
+graphs of different sizes and is designed to provide input files for broad
+range of graph-based research applications, including but not limited to
+testing, benchmarking and performance-analysis of graph processing frameworks.
+Pyrgg target audiences are computer scientists who study graph algorithms and
+graph processing frameworks.
    Open Hub  [https://www.openhub.net/p/pyrgg/widgets/project_thin_badge.gif]
 PyPI Counter                          [http://pepy.tech/badge/pyrgg]
 Github Stars          [https://img.shields.io/github/stars/sepandhaghighi/
                               pyrgg.svg?style=social&label=Stars]
 Branch                      master                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI          pyrgg/workflows/CI/                 pyrgg/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [codebeat_badge] [CodeFactor]
              11ec048bcd594d84997380b64d2d4add]
-## Installation ### Source Code - Download [Version 1.3](https://github.com/
-sepandhaghighi/pyrgg/archive/v1.3.zip) or [Latest Source ](https://github.com/
-sepandhaghighi/pyrgg/archive/dev.zip) - `pip install -r requirements.txt` or
-`pip3 install -r requirements.txt` (Need root access) - `python3 setup.py
-install` or `python setup.py install` (Need root access) ### PyPI - Check
-[Python Packaging User Guide](https://packaging.python.org/installing/) - `pip
-install pyrgg==1.3` or `pip3 install pyrgg==1.3` (Need root access) ### Conda -
-Check [Conda Managing Package](https://conda.io) - `conda install -
-c sepandhaghighi pyrgg` (Need root access) ### Exe Version (Only Windows) -
-Download [Exe-Version 1.3](https://github.com/sepandhaghighi/pyrgg/releases/
-download/v1.3/PYRGG-1.3.exe) - Run `PYRGG-1.3.exe` ### System Requirements
-Pyrgg will likely run on a modern dual core PC. Typical configuration is: -
-Dual Core CPU (2.0 Ghz+) - 4GB of RAM Note that it may run on lower end
-equipment though good performance is not guaranteed. ## Usage - Open `CMD`
-(Windows) or `Terminal` (UNIX) - Run `pyrgg` or `python -m pyrgg` (or run
-`PYRGG.exe`) - Enter data
+## Installation ### PyPI - Check [Python Packaging User Guide](https://
+packaging.python.org/installing/) - `pip install pyrgg==1.4` (Need root access)
+### Source Code - Download [Version 1.4](https://github.com/sepandhaghighi/
+pyrgg/archive/v1.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/
+pyrgg/archive/dev.zip) - `pip install .` (Need root access) ### Conda - Check
+[Conda Managing Package](https://conda.io) - `conda install -c sepandhaghighi
+pyrgg` (Need root access) ### Exe Version (Only Windows) - Download [Exe-
+Version 1.4](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.4/
+PYRGG-1.4.exe) - Run `PYRGG-1.4.exe` ### System Requirements Pyrgg will likely
+run on a modern dual core PC. Typical configuration is: - Dual Core CPU (2.0
+Ghz+) - 4GB of RAM Note that it may run on lower end equipment though good
+performance is not guaranteed. ## Usage - Open `CMD` (Windows) or `Terminal`
+(UNIX) - Run `pyrgg` or `python -m pyrgg` (or run `PYRGG.exe`) - Enter data
                      [https://asciinema.org/a/539844.svg]
 ## Supported Formats - [DIMACS(.gr)](http://www.diag.uniroma1.it/challenge9/
 format.shtml) ``` p sp   a    . . . a    ``` * [Sample 1](https://
 www.dropbox.com/s/i80tnwuuv4iyqet/100.gr.gz?dl=0) (100 Vertices , 3KB) *
 [Sample 2](https://www.dropbox.com/s/lqk42pwu7o4xauv/1000.gr.gz?dl=0) (1000
 Vertices , 13KB) * [Sample 3](https://www.dropbox.com/s/93dp8cjs6lnu83u/
 1000000.gr.gz?dl=0) (1000000 Vertices , 7MB) * [Sample 4](https://
@@ -174,20 +169,17 @@
 github.com/prathasah/random-modular-network-generator) Generates random graphs
 with tunable strength of community structure - [randomGraph](https://
 github.com/sdghafouri/randomGraph) very simple random graph generator in MATLAB
 - [Graph1](https://github.com/Saptaparni/Graph1) Random Graph Generator with
 Max capacity paths (C++) ## Issues & Bug Reports Just fill an issue and
 describe it. We'll check it ASAP! or send an email to [info@pyrgg.ir](mailto:
 info@pyrgg.ir "info@pyrgg.ir"). You can also join our discord server [Discord
-Channel] ## Dependencies
-           master                  dev
-[Requirements_Status] [Requirements_Status]
-## Citing If you use pyrgg in your research, please cite the [JOSS paper](http:
-//joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg JOSS Paper") ;-
-)
+Channel] ## Citing If you use pyrgg in your research, please cite the [JOSS
+paper](http://joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg
+JOSS Paper") ;-)
 @article{Haghighi2017,
   doi = {10.21105/joss.00331},
   url = {https://doi.org/10.21105/joss.00331},
   year  = {2017},
   month = {sep},
   publisher = {The Open Journal},
   volume = {2},
@@ -224,15 +216,16 @@
      and Applied Mathematics, 2004.
      12- Zhong, Jianlong, and Bingsheng He. "An overview of medusa:
      simplified graph processing on gpus." ACM SIGPLAN Notices 47.8
      (2012): 283-284.
      13- Ellson, John, et al. "Graphviz and dynagraphâstatic and dynamic
      graph drawing tools." Graph drawing software. Springer, Berlin,
      Heidelberg, 2004. 127-148.
-## Show Your Support
+* Logo designed by [Zahra Mobasher](https://www.instagram.com/
+littleblackoyster) ## Show Your Support
 **** Star This Repo ****
  Give a â­ï¸ if this project helped you!
 **** Donate to Our Project ****
 *** Bitcoin ***
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 *** Ethereum ***
 0xcD4Db18B6664A9662123D4307B074aE968535388
@@ -251,69 +244,73 @@
 *** Dash ***
 Xd3Yn2qZJ7VE8nbKw2fS98aLxR5M6WUU3s
 *** Stellar ***
  GALPOLPISRHIYHLQER2TLJRGUSZH52RYDK6C3HIU4PSMNAV65Q36EGNL
 *** Zilliqa ***
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 *** Coffeete ***
-[http://www.coffeete.ir/images/buttons/lemonchiffon.png]
- # Changelog All notable changes to this project will be documented in this
-file. The format is based on [Keep a Changelog](http://keepachangelog.com/en/
-1.0.0/) and this project adheres to [Semantic Versioning](http://semver.org/
-spec/v2.0.0.html). ## [Unreleased] ## [1.3] - 2022-11-30 ### Added - Graphviz
-(DOT) format ### Changed - [asciinema](https://asciinema.org) instruction video
-updated - Test system modified - `README.md` modified - `Python 3.11` added to
-`test.yml` - CLI mode updated - `dev-requirements.txt` updated - To-do list
-moved to `TODO.md` ## [1.2] - 2022-09-07 ### Added - Anaconda workflow -
-Discord badge ### Changed - Menu optimized - Docstrings modified - `branch_gen`
-function modified - `edge_gen` function modified - `precision` and `min_edge`
-parameters added to `branch_gen` function - `random_edge` parameter removed
-from `branch_gen` function - Test system modified - `AUTHORS.md` updated -
-License updated - `README.md` modified - `Python 3.10` added to `test.yml` ###
-Removed - `sign_gen` function - `random_edge_limits` function ## [1.1] - 2021-
-06-09 ### Added - `requirements-splitter.py` - `is_weighted` function -
-`_write_properties_to_json` function - `PYRGG_TEST_MODE` parameter ### Changed
-- Test system modified - JSON, YAML and Pickle formats value changed from
-`string` to `number` - `properties` section added to JSON, YAML and Pickle
-formats - `_write_to_json` function renamed to `_write_data_to_json` - `logger`
-function modified - `time_convert` function modified - `branch_gen` function
-modified - References updated ## [1.0] - 2021-01-11 ### Added - Number of files
-option ### Changed - All flags type changed to `bool` - Menu optimized - The
-`logger` function enhanced. - Time format in the `logger` changed to `%Y-%m-%d
-%H:%M:%S` - `dl_maker` function modified - `tgf_maker` function modified -
-`gdf_maker` function modified - `run` function modified ## [0.9] - 2020-10-07
-### Added - GEXF format - Float weight support - `tox.ini` ### Changed - Menu
-optimized - `pyrgg.py` renamed to `graph_gen.py` - Other functions moved to
-`functions.py` - Test system modified - `params.py` refactored - `graph_gen.py`
-refactored - `functions.py` refactored - `weight_str_to_number` function
-renamed to `convert_str_to_number` - `branch_gen` function bugs fixed -
-`input_filter` function bug fixed - `gl_maker` function bug fixed -
-`CONTRIBUTING.md` updated - `AUTHORS.md` updated ### Removed - `print_test`
-function - `left_justify` function - `justify` function - `zero_insert`
-function ## [0.8] - 2020-08-19 ### Added - GDF format - GML format ### Changed
-- CLI snapshots updated - `AUTHORS.md` updated ## [0.7] - 2020-08-07 ### Added
-- Graph Line format ### Changed - Menu optimized ## [0.6] - 2020-07-24 ###
-Added - Matrix Market format ### Changed - `json_maker` function optimized -
-`dl_maker` function optimized - `tgf_maker` function optimized - `lp_maker`
-function optimized ## [0.5] - 2020-07-01 ### Added - TSV format - Multigraph
-control ### Changed - `branch_gen` function modified - Website changed to
-[https://www.pyrgg.ir](https://www.pyrgg.ir) ## [0.4] - 2020-06-17 ### Added -
-Self loop control - Github action ### Changed - `appveyor.yml` updated ## [0.3]
-- 2019-11-29 ### Added - `__version__` variable - `CHANGELOG.md` - `dev-
-requirements.txt` - `requirements.txt` - `CODE_OF_CONDUCT.md` -
-`ISSUE_TEMPLATE.md` - `PULL_REQUEST_TEMPLATE.md` - `CONTRIBUTING.md` -
-`version_check.py` - `pyrgg_profile.py` - Unweighted graph - Undirected graph -
-Exe version ### Changed - Test system modified - `README.md` modified -
-Docstrings modified - `get_input` function modified - `edge_gen` function
-modified - Parameters moved to `params.py` ## [0.2] - 2017-09-20 ### Added -
-CSV format - YAML format - Weighted edge list format (WEL) - ASP format -
-Trivial graph format (TGF) - UCINET DL format - Pickle format ## [0.1] - 2017-
-08-19 ### Added - DIMACS format - JSON format - README [Unreleased]: https://
-github.com/sepandhaghighi/pyrgg/compare/v1.3...dev [1.3]: https://github.com/
-sepandhaghighi/pyrgg/compare/v1.2...v1.3 [1.2]: https://github.com/
+[http://www.coffeete.ir/images/buttons/lemonchiffon.png] # Changelog All
+notable changes to this project will be documented in this file. The format is
+based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
+project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
+## [Unreleased] ## [1.4] - 2023-07-06 ### Added - `check_for_config` function -
+`load_config` function - `save_config` function ### Changed - `README.md`
+modified - Logo changed - `codecov` removed from `dev-requirements.txt` - Test
+system modified - Error messages updated ## [1.3] - 2022-11-30 ### Added -
+Graphviz(DOT) format ### Changed - [asciinema](https://asciinema.org)
+instruction video updated - Test system modified - `README.md` modified -
+`Python 3.11` added to `test.yml` - CLI mode updated - `dev-requirements.txt`
+updated - To-do list moved to `TODO.md` ## [1.2] - 2022-09-07 ### Added -
+Anaconda workflow - Discord badge ### Changed - Menu optimized - Docstrings
+modified - `branch_gen` function modified - `edge_gen` function modified -
+`precision` and `min_edge` parameters added to `branch_gen` function -
+`random_edge` parameter removed from `branch_gen` function - Test system
+modified - `AUTHORS.md` updated - License updated - `README.md` modified -
+`Python 3.10` added to `test.yml` ### Removed - `sign_gen` function -
+`random_edge_limits` function ## [1.1] - 2021-06-09 ### Added - `requirements-
+splitter.py` - `is_weighted` function - `_write_properties_to_json` function -
+`PYRGG_TEST_MODE` parameter ### Changed - Test system modified - JSON, YAML and
+Pickle formats value changed from `string` to `number` - `properties` section
+added to JSON, YAML and Pickle formats - `_write_to_json` function renamed to
+`_write_data_to_json` - `logger` function modified - `time_convert` function
+modified - `branch_gen` function modified - References updated ## [1.0] - 2021-
+01-11 ### Added - Number of files option ### Changed - All flags type changed
+to `bool` - Menu optimized - The `logger` function enhanced. - Time format in
+the `logger` changed to `%Y-%m-%d %H:%M:%S` - `dl_maker` function modified -
+`tgf_maker` function modified - `gdf_maker` function modified - `run` function
+modified ## [0.9] - 2020-10-07 ### Added - GEXF format - Float weight support -
+`tox.ini` ### Changed - Menu optimized - `pyrgg.py` renamed to `graph_gen.py` -
+Other functions moved to `functions.py` - Test system modified - `params.py`
+refactored - `graph_gen.py` refactored - `functions.py` refactored -
+`weight_str_to_number` function renamed to `convert_str_to_number` -
+`branch_gen` function bugs fixed - `input_filter` function bug fixed -
+`gl_maker` function bug fixed - `CONTRIBUTING.md` updated - `AUTHORS.md`
+updated ### Removed - `print_test` function - `left_justify` function -
+`justify` function - `zero_insert` function ## [0.8] - 2020-08-19 ### Added -
+GDF format - GML format ### Changed - CLI snapshots updated - `AUTHORS.md`
+updated ## [0.7] - 2020-08-07 ### Added - Graph Line format ### Changed - Menu
+optimized ## [0.6] - 2020-07-24 ### Added - Matrix Market format ### Changed -
+`json_maker` function optimized - `dl_maker` function optimized - `tgf_maker`
+function optimized - `lp_maker` function optimized ## [0.5] - 2020-07-01 ###
+Added - TSV format - Multigraph control ### Changed - `branch_gen` function
+modified - Website changed to [https://www.pyrgg.ir](https://www.pyrgg.ir) ##
+[0.4] - 2020-06-17 ### Added - Self loop control - Github action ### Changed -
+`appveyor.yml` updated ## [0.3] - 2019-11-29 ### Added - `__version__` variable
+- `CHANGELOG.md` - `dev-requirements.txt` - `requirements.txt` -
+`CODE_OF_CONDUCT.md` - `ISSUE_TEMPLATE.md` - `PULL_REQUEST_TEMPLATE.md` -
+`CONTRIBUTING.md` - `version_check.py` - `pyrgg_profile.py` - Unweighted graph
+- Undirected graph - Exe version ### Changed - Test system modified -
+`README.md` modified - Docstrings modified - `get_input` function modified -
+`edge_gen` function modified - Parameters moved to `params.py` ## [0.2] - 2017-
+09-20 ### Added - CSV format - YAML format - Weighted edge list format (WEL) -
+ASP format - Trivial graph format (TGF) - UCINET DL format - Pickle format ##
+[0.1] - 2017-08-19 ### Added - DIMACS format - JSON format - README
+[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.4...dev [1.4]:
+https://github.com/sepandhaghighi/pyrgg/compare/v1.3...v1.4 [1.3]: https://
+github.com/sepandhaghighi/pyrgg/compare/v1.2...v1.3 [1.2]: https://github.com/
 sepandhaghighi/pyrgg/compare/v1.1...v1.2 [1.1]: https://github.com/
 sepandhaghighi/pyrgg/compare/v1.0...v1.1 [1.0]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.9...v1.0 [0.9]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.8...v0.9 [0.8]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.7...v0.8 [0.7]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.6...v0.7 [0.6]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.5...v0.6 [0.5]: https://github.com/
```

### Comparing `pyrgg-1.3/README.md` & `pyrgg-1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-
-							
-
-
 <div align="center">
-<img src="http://www.shaghighi.ir/pyrgg/images/pyrgg-logo.png" height=240px width=320px>
-<hr/>
-<h1>Random Graph Generator</h1>
-
-<a href="http://www.shaghighi.ir/pyrgg"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=website"></a>
-<a href="https://badge.fury.io/py/pyrgg"><img src="https://badge.fury.io/py/pyrgg.svg" alt="PyPI version" height="18"></a>
-<a href="https://anaconda.org/sepandhaghighi/pyrgg"><img src="https://anaconda.org/sepandhaghighi/pyrgg/badges/version.svg"></a>
-<a href="https://codecov.io/gh/sepandhaghighi/pyrgg">
-  <img src="https://codecov.io/gh/sepandhaghighi/pyrgg/branch/master/graph/badge.svg" alt="Codecov" /></a>
-<a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
-<a href="https://discord.gg/dfYAWVMaCW">
-  <img src="https://img.shields.io/discord/1013411447130308669.svg" alt="Discord Channel">
-</a>
+	<img src="https://github.com/sepandhaghighi/pyrgg/raw/master/otherfile/logo.png" width="450">
+	<h1>PyRGG: Python Random Graph Generator</h1>
+	<a href="http://www.shaghighi.ir/pyrgg">
+		<img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=website">
+	</a>
+	<a href="https://badge.fury.io/py/pyrgg">
+		<img src="https://badge.fury.io/py/pyrgg.svg" alt="PyPI version" height="18">
+	</a>
+	<a href="https://anaconda.org/sepandhaghighi/pyrgg">
+		<img src="https://anaconda.org/sepandhaghighi/pyrgg/badges/version.svg">
+	</a>
+	<a href="https://codecov.io/gh/sepandhaghighi/pyrgg">
+  		<img src="https://codecov.io/gh/sepandhaghighi/pyrgg/branch/master/graph/badge.svg" alt="Codecov">
+	</a>
+	<a href="https://www.python.org/">
+		<img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3">
+	</a>
+	<a href="https://discord.gg/dfYAWVMaCW">
+  		<img src="https://img.shields.io/discord/1013411447130308669.svg" alt="Discord Channel">
+	</a>
 </div>	
 
-----------
 ## Table of Contents					
    * [Overview](https://github.com/sepandhaghighi/pyrgg#overview)
    * [Installation](https://github.com/sepandhaghighi/pyrgg#installation)
    * [Usage](https://github.com/sepandhaghighi/pyrgg#usage)
    * [Supported Formats](https://github.com/sepandhaghighi/pyrgg#supported-formats)
    * [Example of Usage](https://github.com/sepandhaghighi/pyrgg#example-of-usage)
    * [Similar Works](https://github.com/sepandhaghighi/pyrgg#similar-works)
    * [Issues & Bug Reports](https://github.com/sepandhaghighi/pyrgg#issues--bug-reports)
-   * [Dependencies](https://github.com/sepandhaghighi/pyrgg#dependencies)
    * [Contribution](https://github.com/sepandhaghighi/pyrgg/blob/master/.github/CONTRIBUTING.md)
    * [References](https://github.com/sepandhaghighi/pyrgg#references)
    * [Citing](https://github.com/sepandhaghighi/pyrgg#citing)
    * [Authors](https://github.com/sepandhaghighi/pyrgg/blob/master/AUTHORS.md)
    * [License](https://github.com/sepandhaghighi/pyrgg/blob/master/LICENSE)
    * [Show Your Support](https://github.com/sepandhaghighi/pyrgg#show-your-support)
    * [Todo](https://github.com/sepandhaghighi/pyrgg/blob/master/TODO.md)
@@ -82,32 +83,31 @@
 		<td align="center"><a href="https://www.codefactor.io/repository/github/sepandhaghighi/pyrgg"><img src="https://www.codefactor.io/repository/github/sepandhaghighi/pyrgg/badge" alt="CodeFactor" /></a></td>	
 	</tr>
 </table>
 
 
 ## Installation		
 
-### Source Code
-- Download [Version 1.3](https://github.com/sepandhaghighi/pyrgg/archive/v1.3.zip) or [Latest Source ](https://github.com/sepandhaghighi/pyrgg/archive/dev.zip)
-- `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
-- `python3 setup.py install` or `python setup.py install` (Need root access)				
-
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install pyrgg==1.3` or `pip3 install pyrgg==1.3` (Need root access)							
+- `pip install pyrgg==1.4` (Need root access)							
+
+### Source Code
+- Download [Version 1.4](https://github.com/sepandhaghighi/pyrgg/archive/v1.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/pyrgg/archive/dev.zip)
+- `pip install .` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io)
 - `conda install -c sepandhaghighi pyrgg` (Need root access)	
 
 ### Exe Version (Only Windows)
-- Download [Exe-Version 1.3](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.3/PYRGG-1.3.exe)
-- Run `PYRGG-1.3.exe`
+- Download [Exe-Version 1.4](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.4/PYRGG-1.4.exe)
+- Run `PYRGG-1.4.exe`
 
 ### System Requirements
 Pyrgg will likely run on a modern dual core PC. Typical configuration is:
 
 - Dual Core CPU (2.0 Ghz+)
 - 4GB of RAM
 
@@ -468,27 +468,14 @@
 
 You can also join our discord server			
 
 <a href="https://discord.gg/dfYAWVMaCW">
   <img src="https://img.shields.io/discord/1013411447130308669.svg?style=for-the-badge" alt="Discord Channel">
 </a>
 
-## Dependencies
-
-<table>
-	<tr> 
-		<td align="center">master</td>	
-		<td align="center">dev</td>	
-	</tr>
-	<tr>
-		<td align="center"><a href="https://requires.io/github/sepandhaghighi/pyrgg/requirements/?branch=master"><img src="https://requires.io/github/sepandhaghighi/pyrgg/requirements.svg?branch=master" alt="Requirements Status" /></a></td>
-		<td align="center"><a href="https://requires.io/github/sepandhaghighi/pyrgg/requirements/?branch=dev"><img src="https://requires.io/github/sepandhaghighi/pyrgg/requirements.svg?branch=dev" alt="Requirements Status" /></a></td>
-	</tr>
-</table>
-
 
 ## Citing
 
 If you use pyrgg in your research, please cite the [JOSS paper](http://joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg JOSS Paper") ;-)
 
 <pre>
 @article{Haghighi2017,
@@ -541,14 +528,17 @@
 <blockquote>10- Skiena, Steven S. The algorithm design manual. Springer International Publishing, 2020. </blockquote>
 
 <blockquote>11- Chakrabarti, Deepayan, Yiping Zhan, and Christos Faloutsos. "R-MAT: A recursive model for graph mining." Proceedings of the 2004 SIAM International Conference on Data Mining. Society for Industrial and Applied Mathematics, 2004. </blockquote>
 
 <blockquote>12- Zhong, Jianlong, and Bingsheng He. "An overview of medusa: simplified graph processing on gpus." ACM SIGPLAN Notices 47.8 (2012): 283-284.</blockquote>
 
 <blockquote>13- Ellson, John, et al. "Graphviz and dynagraph—static and dynamic graph drawing tools." Graph drawing software. Springer, Berlin, Heidelberg, 2004. 127-148.</blockquote>
+
+
+* Logo designed by [Zahra Mobasher](https://www.instagram.com/littleblackoyster)	
 					
  
 ## Show Your Support
 								
 <h3>Star This Repo</h3>					
 
 Give a ⭐️ if this project helped you!
@@ -576,8 +566,9 @@
 <h4>Stellar</h4>		
 GALPOLPISRHIYHLQER2TLJRGUSZH52RYDK6C3HIU4PSMNAV65Q36EGNL
 <h4>Zilliqa</h4>
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 <h4>Coffeete</h4>
 <a href="http://www.coffeete.ir/opensource">
 <img src="http://www.coffeete.ir/images/buttons/lemonchiffon.png" style="width:260px;" />
-</a>	
+</a>
+
```

#### html2text {}

```diff
@@ -1,66 +1,61 @@
-            [http://www.shaghighi.ir/pyrgg/images/pyrgg-logo.png]
-===============================================================================
-                     ****** Random Graph Generator ******
+    [https://github.com/sepandhaghighi/pyrgg/raw/master/otherfile/logo.png]
+              ****** PyRGG: Python Random Graph Generator ******
             [https://img.shields.io/website-up-down-green-red/http/
       shields.io.svg?label=website] [PyPI_version] [https://anaconda.org/
    sepandhaghighi/pyrgg/badges/version.svg] [Codecov] [built_with_Python3]
                                [Discord_Channel]
- ---------- ## Table of Contents * [Overview](https://github.com/
-sepandhaghighi/pyrgg#overview) * [Installation](https://github.com/
-sepandhaghighi/pyrgg#installation) * [Usage](https://github.com/sepandhaghighi/
-pyrgg#usage) * [Supported Formats](https://github.com/sepandhaghighi/
-pyrgg#supported-formats) * [Example of Usage](https://github.com/
-sepandhaghighi/pyrgg#example-of-usage) * [Similar Works](https://github.com/
-sepandhaghighi/pyrgg#similar-works) * [Issues & Bug Reports](https://
-github.com/sepandhaghighi/pyrgg#issues--bug-reports) * [Dependencies](https://
-github.com/sepandhaghighi/pyrgg#dependencies) * [Contribution](https://
-github.com/sepandhaghighi/pyrgg/blob/master/.github/CONTRIBUTING.md) *
-[References](https://github.com/sepandhaghighi/pyrgg#references) * [Citing]
-(https://github.com/sepandhaghighi/pyrgg#citing) * [Authors](https://
-github.com/sepandhaghighi/pyrgg/blob/master/AUTHORS.md) * [License](https://
-github.com/sepandhaghighi/pyrgg/blob/master/LICENSE) * [Show Your Support]
-(https://github.com/sepandhaghighi/pyrgg#show-your-support) * [Todo](https://
-github.com/sepandhaghighi/pyrgg/blob/master/TODO.md) * [Changelog](https://
-github.com/sepandhaghighi/pyrgg/blob/master/CHANGELOG.md) * [Code of Conduct]
-(https://github.com/sepandhaghighi/pyrgg/blob/master/.github/
-CODE_OF_CONDUCT.md) ## Overview Pyrgg is an easy-to-use synthetic random graph
-generator written in Python which supports various graph file formats including
-DIMACS_.gr files. Pyrgg has the ability to generate graphs of different sizes
-and is designed to provide input files for broad range of graph-based research
-applications, including but not limited to testing, benchmarking and
-performance-analysis of graph processing frameworks. Pyrgg target audiences are
-computer scientists who study graph algorithms and graph processing frameworks.
+ ## Table of Contents * [Overview](https://github.com/sepandhaghighi/
+pyrgg#overview) * [Installation](https://github.com/sepandhaghighi/
+pyrgg#installation) * [Usage](https://github.com/sepandhaghighi/pyrgg#usage) *
+[Supported Formats](https://github.com/sepandhaghighi/pyrgg#supported-formats)
+* [Example of Usage](https://github.com/sepandhaghighi/pyrgg#example-of-usage)
+* [Similar Works](https://github.com/sepandhaghighi/pyrgg#similar-works) *
+[Issues & Bug Reports](https://github.com/sepandhaghighi/pyrgg#issues--bug-
+reports) * [Contribution](https://github.com/sepandhaghighi/pyrgg/blob/
+master/.github/CONTRIBUTING.md) * [References](https://github.com/
+sepandhaghighi/pyrgg#references) * [Citing](https://github.com/sepandhaghighi/
+pyrgg#citing) * [Authors](https://github.com/sepandhaghighi/pyrgg/blob/master/
+AUTHORS.md) * [License](https://github.com/sepandhaghighi/pyrgg/blob/master/
+LICENSE) * [Show Your Support](https://github.com/sepandhaghighi/pyrgg#show-
+your-support) * [Todo](https://github.com/sepandhaghighi/pyrgg/blob/master/
+TODO.md) * [Changelog](https://github.com/sepandhaghighi/pyrgg/blob/master/
+CHANGELOG.md) * [Code of Conduct](https://github.com/sepandhaghighi/pyrgg/blob/
+master/.github/CODE_OF_CONDUCT.md) ## Overview Pyrgg is an easy-to-use
+synthetic random graph generator written in Python which supports various graph
+file formats including DIMACS_.gr files. Pyrgg has the ability to generate
+graphs of different sizes and is designed to provide input files for broad
+range of graph-based research applications, including but not limited to
+testing, benchmarking and performance-analysis of graph processing frameworks.
+Pyrgg target audiences are computer scientists who study graph algorithms and
+graph processing frameworks.
    Open Hub  [https://www.openhub.net/p/pyrgg/widgets/project_thin_badge.gif]
 PyPI Counter                          [http://pepy.tech/badge/pyrgg]
 Github Stars          [https://img.shields.io/github/stars/sepandhaghighi/
                               pyrgg.svg?style=social&label=Stars]
 Branch                      master                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI          pyrgg/workflows/CI/                 pyrgg/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [codebeat_badge] [CodeFactor]
              11ec048bcd594d84997380b64d2d4add]
-## Installation ### Source Code - Download [Version 1.3](https://github.com/
-sepandhaghighi/pyrgg/archive/v1.3.zip) or [Latest Source ](https://github.com/
-sepandhaghighi/pyrgg/archive/dev.zip) - `pip install -r requirements.txt` or
-`pip3 install -r requirements.txt` (Need root access) - `python3 setup.py
-install` or `python setup.py install` (Need root access) ### PyPI - Check
-[Python Packaging User Guide](https://packaging.python.org/installing/) - `pip
-install pyrgg==1.3` or `pip3 install pyrgg==1.3` (Need root access) ### Conda -
-Check [Conda Managing Package](https://conda.io) - `conda install -
-c sepandhaghighi pyrgg` (Need root access) ### Exe Version (Only Windows) -
-Download [Exe-Version 1.3](https://github.com/sepandhaghighi/pyrgg/releases/
-download/v1.3/PYRGG-1.3.exe) - Run `PYRGG-1.3.exe` ### System Requirements
-Pyrgg will likely run on a modern dual core PC. Typical configuration is: -
-Dual Core CPU (2.0 Ghz+) - 4GB of RAM Note that it may run on lower end
-equipment though good performance is not guaranteed. ## Usage - Open `CMD`
-(Windows) or `Terminal` (UNIX) - Run `pyrgg` or `python -m pyrgg` (or run
-`PYRGG.exe`) - Enter data
+## Installation ### PyPI - Check [Python Packaging User Guide](https://
+packaging.python.org/installing/) - `pip install pyrgg==1.4` (Need root access)
+### Source Code - Download [Version 1.4](https://github.com/sepandhaghighi/
+pyrgg/archive/v1.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/
+pyrgg/archive/dev.zip) - `pip install .` (Need root access) ### Conda - Check
+[Conda Managing Package](https://conda.io) - `conda install -c sepandhaghighi
+pyrgg` (Need root access) ### Exe Version (Only Windows) - Download [Exe-
+Version 1.4](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.4/
+PYRGG-1.4.exe) - Run `PYRGG-1.4.exe` ### System Requirements Pyrgg will likely
+run on a modern dual core PC. Typical configuration is: - Dual Core CPU (2.0
+Ghz+) - 4GB of RAM Note that it may run on lower end equipment though good
+performance is not guaranteed. ## Usage - Open `CMD` (Windows) or `Terminal`
+(UNIX) - Run `pyrgg` or `python -m pyrgg` (or run `PYRGG.exe`) - Enter data
                      [https://asciinema.org/a/539844.svg]
 ## Supported Formats - [DIMACS(.gr)](http://www.diag.uniroma1.it/challenge9/
 format.shtml) ``` p sp   a    . . . a    ``` * [Sample 1](https://
 www.dropbox.com/s/i80tnwuuv4iyqet/100.gr.gz?dl=0) (100 Vertices , 3KB) *
 [Sample 2](https://www.dropbox.com/s/lqk42pwu7o4xauv/1000.gr.gz?dl=0) (1000
 Vertices , 13KB) * [Sample 3](https://www.dropbox.com/s/93dp8cjs6lnu83u/
 1000000.gr.gz?dl=0) (1000000 Vertices , 7MB) * [Sample 4](https://
@@ -149,20 +144,17 @@
 github.com/prathasah/random-modular-network-generator) Generates random graphs
 with tunable strength of community structure - [randomGraph](https://
 github.com/sdghafouri/randomGraph) very simple random graph generator in MATLAB
 - [Graph1](https://github.com/Saptaparni/Graph1) Random Graph Generator with
 Max capacity paths (C++) ## Issues & Bug Reports Just fill an issue and
 describe it. We'll check it ASAP! or send an email to [info@pyrgg.ir](mailto:
 info@pyrgg.ir "info@pyrgg.ir"). You can also join our discord server [Discord
-Channel] ## Dependencies
-           master                  dev
-[Requirements_Status] [Requirements_Status]
-## Citing If you use pyrgg in your research, please cite the [JOSS paper](http:
-//joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg JOSS Paper") ;-
-)
+Channel] ## Citing If you use pyrgg in your research, please cite the [JOSS
+paper](http://joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg
+JOSS Paper") ;-)
 @article{Haghighi2017,
   doi = {10.21105/joss.00331},
   url = {https://doi.org/10.21105/joss.00331},
   year  = {2017},
   month = {sep},
   publisher = {The Open Journal},
   volume = {2},
@@ -199,15 +191,16 @@
      and Applied Mathematics, 2004.
      12- Zhong, Jianlong, and Bingsheng He. "An overview of medusa:
      simplified graph processing on gpus." ACM SIGPLAN Notices 47.8
      (2012): 283-284.
      13- Ellson, John, et al. "Graphviz and dynagraphâstatic and dynamic
      graph drawing tools." Graph drawing software. Springer, Berlin,
      Heidelberg, 2004. 127-148.
-## Show Your Support
+* Logo designed by [Zahra Mobasher](https://www.instagram.com/
+littleblackoyster) ## Show Your Support
 **** Star This Repo ****
  Give a â­ï¸ if this project helped you!
 **** Donate to Our Project ****
 *** Bitcoin ***
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 *** Ethereum ***
 0xcD4Db18B6664A9662123D4307B074aE968535388
```

### Comparing `pyrgg-1.3/TODO.md` & `pyrgg-1.4/TODO.md`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/paper/10.21105.joss.00331.pdf` & `pyrgg-1.4/paper/10.21105.joss.00331.pdf`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/paper/paper.bib` & `pyrgg-1.4/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/paper/paper.md` & `pyrgg-1.4/paper/paper.md`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/pyrgg/__main__.py` & `pyrgg-1.4/pyrgg/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -83,23 +83,29 @@
         multigraph,
         self_loop,
         max_weight,
         min_weight,
         elapsed_time_format)
 
 
-def run():
+def run(input_dict=None):
     """
     Run proper converter.
 
+    :param input_dict: input data
+    :type input_dict: dict
     :return: None
     """
-    input_dict = get_input()
+    if input_dict is None:
+        input_dict = get_input()
+        if input_dict["config"] is True:
+            print("Config --> " + save_config(input_dict))
     file_name = input_dict["file_name"]
     number_of_files = input_dict["number_of_files"]
+    line(40)
     for i in range(number_of_files):
         print("Generating {0} from {1}".format(i + 1, number_of_files))
         file_name_temp = file_name
         if number_of_files > 1:
             file_name_temp = file_name + "_" + str(i + 1)
         gen_graph(input_dict, file_name_temp)
         line(40)
@@ -109,14 +115,15 @@
     """
     CLI main function.
 
     :return: None
     """
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', help='version', nargs="?", const=1)
+    parser.add_argument('--config', help='config')
     parser.add_argument('test', help='test', nargs="?", const=1)
     args = parser.parse_args()
     if args.version:
         print(PYRGG_VERSION)
     elif args.test:
         print("Testing ...")
         error_flag = doctest.testfile("test.py", verbose=False)[0]
@@ -124,16 +131,21 @@
             print("Done!")
         sys.exit(error_flag)
     else:
         tprint("Pyrgg", "larry3d")
         tprint("v" + PYRGG_VERSION)
         description_print()
         EXIT_FLAG = False
+        input_dict = None
         while not EXIT_FLAG:
-            run()
+            if args.config:
+                input_dict = load_config(args.config)
+            else:
+                input_dict = check_for_config()
+            run(input_dict)
             INPUTINDEX = str(
                 input("Press [R] to restart Pyrgg or any other key to exit."))
             if INPUTINDEX.upper() != "R":
                 EXIT_FLAG = True
 
 
 if __name__ == "__main__":
```

### Comparing `pyrgg-1.3/pyrgg/functions.py` & `pyrgg-1.4/pyrgg/functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """Pyrgg functions module."""
 import datetime
 from json import loads as json_loads
+from json import dump as json_dump
 import os
 from pickle import dump as pickle_dump
 from random import randint, uniform, choice
 from textwrap import fill
 from yaml import safe_dump as yaml_dump
 import pyrgg.params
 
@@ -79,28 +80,29 @@
     :param string: input string
     :type string: str
     :return: bool
     """
     return bool(int(string))
 
 
-MENU_ITEM_CONVERTORS = {
+ITEM_CONVERTORS = {
     "file_name": lambda x: x,
     "output_format": int,
     "weight": convert_str_to_bool,
     "vertices": int,
     "number_of_files": int,
     "max_weight": convert_str_to_number,
     "min_weight": convert_str_to_number,
     "min_edge": int,
     "max_edge": int,
     "sign": convert_str_to_bool,
     "direct": convert_str_to_bool,
     "self_loop": convert_str_to_bool,
     "multigraph": convert_str_to_bool,
+    "config": convert_str_to_bool,
 }
 
 
 def description_print():
     """
     Print justified description for overview in console.
 
@@ -117,15 +119,15 @@
 def line(num=11, char="#"):
     """
     Print line of char.
 
     :param num: number of character in this line
     :type num : int
     :param char: character
-    :type char : str
+    :type char: str
     :return: None
     """
     print(char * num)
 
 
 def convert_bytes(num):
     """
@@ -283,16 +285,16 @@
     return filtered_dict
 
 
 def get_input(input_func=input):
     """
     Get input from user and return as dictionary.
 
-    :param input_func : input function
-    :type input_func : function object
+    :param input_func: input function
+    :type input_func: function object
     :return: inputs as dict
     """
     result_dict = {
         "file_name": "",
         "number_of_files": 1,
         "vertices": 0,
         "max_weight": 1,
@@ -301,36 +303,37 @@
         "max_edge": 0,
         "sign": True,
         "output_format": 1,
         "weight": True,
         "direct": True,
         "self_loop": True,
         "multigraph": False,
+        "config": False,
     }
 
     result_dict = _update_using_first_menu(result_dict, input_func)
     result_dict = _update_using_second_menu(result_dict, input_func)
     return input_filter(result_dict)
 
 
 def _update_using_first_menu(result_dict, input_func):
     """
     Update result_dict using user input from the first menu.
 
     :param result_dict: result data
     :type result_dict: dict
-    :param input_func : input function
-    :type input_func : function object
+    :param input_func: input function
+    :type input_func: function object
     :return: result_dict as dict
     """
     MENU_ITEMS_KEYS1 = sorted(list(pyrgg.params.MENU_ITEMS1.keys()))
     for item in MENU_ITEMS_KEYS1:
         while True:
             try:
-                result_dict[item] = MENU_ITEM_CONVERTORS[item](
+                result_dict[item] = ITEM_CONVERTORS[item](
                     input_func(pyrgg.params.MENU_ITEMS1[item])
                 )
             except Exception:
                 print(pyrgg.params.PYRGG_INPUT_ERROR_MESSAGE)
             else:
                 break
     return result_dict
@@ -338,27 +341,27 @@
 
 def _update_using_second_menu(result_dict, input_func):
     """
     Update result_dict using user input from the second menu.
 
     :param result_dict: result data
     :type result_dict: dict
-    :param input_func : input function
-    :type input_func : function object
+    :param input_func: input function
+    :type input_func: function object
     :return: result_dict as dict
     """
     MENU_ITEMS_KEYS2 = sorted(list(pyrgg.params.MENU_ITEMS2.keys()))
     for index in MENU_ITEMS_KEYS2:
         item1 = pyrgg.params.MENU_ITEMS2[index][0]
         item2 = pyrgg.params.MENU_ITEMS2[index][1]
         if not result_dict["weight"] and item1 in ["max_weight", "min_weight"]:
             continue
         while True:
             try:
-                result_dict[item1] = MENU_ITEM_CONVERTORS[item1](
+                result_dict[item1] = ITEM_CONVERTORS[item1](
                     input_func(item2)
                 )
             except Exception:
                 print(pyrgg.params.PYRGG_INPUT_ERROR_MESSAGE)
             else:
                 break
     return result_dict
@@ -577,15 +580,15 @@
     """
     try:
         with open(filename + ".json", "r") as json_file:
             json_data = json_loads(json_file.read())
             with open(filename + ".yaml", "w") as yaml_file:
                 yaml_dump(json_data, yaml_file, default_flow_style=False)
     except FileNotFoundError:
-        print(pyrgg.params.PYRGG_FILE_ERROR_MESSAGE)
+        print(pyrgg.params.PYRGG_YAML_ERROR_MESSAGE)
 
 
 def json_to_pickle(filename):
     """
     Convert json file to pickle file.
 
     :param filename: filename
@@ -594,8 +597,86 @@
     """
     try:
         with open(filename + ".json", "r") as json_file:
             json_data = json_loads(json_file.read())
             with open(filename + ".p", "wb") as pickle_file:
                 pickle_dump(json_data, pickle_file)
     except FileNotFoundError:
-        print(pyrgg.params.PYRGG_FILE_ERROR_MESSAGE)
+        print(pyrgg.params.PYRGG_PICKLE_ERROR_MESSAGE)
+
+
+def save_config(input_dict):
+    """
+    Save input_dict as the generation config.
+
+    :param input_dict: input data
+    :type input_dict: dict
+    :return: path to file
+    """
+    try:
+        input_dict_temp = input_dict.copy()
+        input_dict_temp["engine"] = "pyrgg"
+        input_dict_temp['pyrgg_version'] = pyrgg.params.PYRGG_VERSION
+        input_dict_temp['output_format'] = pyrgg.params.OUTPUT_FORMAT[input_dict_temp['output_format']]
+        fname = pyrgg.params.CONFIG_FILE_FORMAT.format(input_dict_temp['file_name'])
+        with open(fname, "w") as json_file:
+            json_dump(input_dict_temp, json_file, indent=2)
+        return os.path.abspath(fname)
+    except BaseException:
+        print(pyrgg.params.PYRGG_CONFIG_SAVE_ERROR_MESSAGE)
+
+
+def load_config(path):
+    """
+    Load config based on given path.
+
+    :param path: path to config file
+    :type path: str
+    :return: input data
+    """
+    try:
+        with open(path, "r") as json_file:
+            config = json_loads(json_file.read())
+            config['output_format'] = pyrgg.params.OUTPUT_FORMAT_INV[config['output_format']]
+            return input_filter(config)
+    except BaseException:
+        print(pyrgg.params.PYRGG_CONFIG_LOAD_ERROR_MESSAGE)
+
+
+def _print_select_config(configs, input_func=input):
+    """
+    Print configs in current directory and get input from user.
+
+    :param configs: configs path
+    :type configs: list
+    :param input_func: input function
+    :type input_func: function object
+    :return: input data
+    """
+    if len(configs) == 0:
+        return None
+    print("Config files detected in current directory are listed below:")
+    for i, config in enumerate(configs):
+        print("[{}] - {}".format(i + 1, config))
+    key = input_func(
+        "Press the config index to load or any other keys to start with new one : ")
+    try:
+        return load_config(configs[int(key) - 1])
+    except BaseException:
+        return None
+
+
+def check_for_config(input_func=input):
+    """
+    Check for config files in source directory.
+
+    :param input_func: input function
+    :type input_func: function object
+    :return: input data
+    """
+    configs = []
+    for filename in os.listdir(pyrgg.params.SOURCE_DIR):
+        file = os.path.join(pyrgg.params.SOURCE_DIR, filename)
+        if os.path.isfile(file) and filename.endswith(
+                pyrgg.params.CONFIG_FILE_FORMAT.format("")):
+            configs.append(file)
+    return _print_select_config(configs, input_func)
```

### Comparing `pyrgg-1.3/pyrgg/graph_gen.py` & `pyrgg-1.4/pyrgg/graph_gen.py`

 * *Files identical despite different names*

### Comparing `pyrgg-1.3/pyrgg/params.py` & `pyrgg-1.4/pyrgg/params.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     2: ["min_edge", "- Min Edge Number (Connected to Each Vertex) : "],
     3: ["max_edge", "- Max Edge Number (Connected to Each Vertex) : "],
     4: ["min_weight", "- Min Weight : "],
     5: ["max_weight", "- Max Weight : "],
     6: ["sign", "- Unsigned[0] or Signed[1]"],
     7: ["direct", "- Undirected[0] or Directed[1]"],
     8: ["self_loop", "- No Self Loop[0] or Self Loop[1]"],
-    9: ["multigraph", "- Simple[0] or Multigraph[1]"]
+    9: ["multigraph", "- Simple[0] or Multigraph[1]"],
+    10: ["config", "- Save config[1] or not[0]"],
 }
 
 
 SUFFIX_MENU = {
     1: ".gr",
     2: ".json",
     3: ".csv",
@@ -58,21 +59,28 @@
     12: ".gl",
     13: ".gdf",
     14: ".gml",
     15: ".gexf",
     16: ".gv"
 }
 
+OUTPUT_FORMAT = {i: output_format[1:].upper()
+                 for i, output_format in SUFFIX_MENU.items()}
 
-PYRGG_VERSION = "1.3"
+OUTPUT_FORMAT_INV = {v: k for k, v in OUTPUT_FORMAT.items()}
+
+
+PYRGG_VERSION = "1.4"
 
 PYRGG_TEST_MODE = False
 
 SOURCE_DIR = os.getcwd()
 
+CONFIG_FILE_FORMAT = "{}.pyrgg.config.json"
+
 PYRGG_LINKS = """
 Webpage : https://www.pyrgg.ir
 Repository : https://github.com/sepandhaghighi/pyrgg
 Paper : https://doi.org/10.21105/joss.00331
 * If you use Pyrgg in your research, please cite our paper
 """
 
@@ -86,19 +94,27 @@
 benchmarking and performance-analysis of graph processing frameworks.
 Pyrgg target audiences are computer scientists
 who study graph algorithms and graph processing frameworks.
 """
 
 PYRGG_DESCRIPTION = fill(_description, width=70)
 
-PYRGG_INPUT_ERROR_MESSAGE = "[Error] Bad Input!"
+PYRGG_INPUT_ERROR_MESSAGE = "[Error] Bad input!"
+
+PYRGG_FILE_ERROR_MESSAGE = "[Error] Bad input file!"
+
+PYRGG_YAML_ERROR_MESSAGE = "[Error] Failed to generate YAML file!"
+
+PYRGG_PICKLE_ERROR_MESSAGE = "[Error] Failed to generate Pickle file!"
+
+PYRGG_LOGGER_ERROR_MESSAGE = "[Error] Logger failed!"
 
-PYRGG_FILE_ERROR_MESSAGE = "[Error] Bad Input File!"
+PYRGG_CONFIG_LOAD_ERROR_MESSAGE = "[Error] Failed to load config file!"
 
-PYRGG_LOGGER_ERROR_MESSAGE = "[Error] Logger Failed!"
+PYRGG_CONFIG_SAVE_ERROR_MESSAGE = "[Error] Failed to save config file!"
 
 PYRGG_LOGGER_TEMPLATE = """{0}
 Filename : {1}
 Vertices : {2}
 Total Edges : {3}
 Max Edge : {4}
 Min Edge : {5}
```

### Comparing `pyrgg-1.3/pyrgg/test.py` & `pyrgg-1.4/pyrgg/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,17 +416,17 @@
 >>> testfile_3_yaml['graph']['edges'][1]['source']
 3
 >>> testfile_3_yaml['graph']['edges'][1]['target']
 76
 >>> testfile_3_yaml['graph']['edges'][1]['weight']
 15
 >>> json_to_yaml('testfile24')
-[Error] Bad Input File!
+[Error] Failed to generate YAML file!
 >>> json_to_pickle('testfile24')
-[Error] Bad Input File!
+[Error] Failed to generate Pickle file!
 >>> json_maker('testfile', 0, 200, 10, 0, 0,True)
 Traceback (most recent call last):
         ...
 TypeError: json_maker() missing 3 required positional arguments: 'direct', 'self_loop', and 'multigraph'
 >>> json_to_pickle('testfile3')
 >>> testfile_3_p=pickle.load( open( 'testfile3.p', 'rb' ) )
 >>> testfile_3_p['graph']['edges'][1]['source']
```

### Comparing `pyrgg-1.3/pyrgg.egg-info/PKG-INFO` & `pyrgg-1.4/pyrgg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrgg
-Version: 1.3
+Version: 1.4
 Summary: Python Random Graph Generator
 Home-page: https://github.com/sepandhaghighi/pyrgg
-Download-URL: https://github.com/sepandhaghighi/pyrgg/tarball/v1.3
+Download-URL: https://github.com/sepandhaghighi/pyrgg/tarball/v1.4
 Author: PyRGG Development Team
 Author-email: info@pyrgg.ir
 License: MIT
 Project-URL: Webpage, https://www.pyrgg.ir
 Project-URL: Source, https://github.com/sepandhaghighi/pyrgg
 Keywords: random graph python3 python generator graph-process generator DIMACS JSON YAML Pickle CSV TSV WEL ASP TGF UCINET
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,44 +36,45 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
-
-							
-
-
 <div align="center">
-<img src="http://www.shaghighi.ir/pyrgg/images/pyrgg-logo.png" height=240px width=320px>
-<hr/>
-<h1>Random Graph Generator</h1>
-
-<a href="http://www.shaghighi.ir/pyrgg"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=website"></a>
-<a href="https://badge.fury.io/py/pyrgg"><img src="https://badge.fury.io/py/pyrgg.svg" alt="PyPI version" height="18"></a>
-<a href="https://anaconda.org/sepandhaghighi/pyrgg"><img src="https://anaconda.org/sepandhaghighi/pyrgg/badges/version.svg"></a>
-<a href="https://codecov.io/gh/sepandhaghighi/pyrgg">
-  <img src="https://codecov.io/gh/sepandhaghighi/pyrgg/branch/master/graph/badge.svg" alt="Codecov" /></a>
-<a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
-<a href="https://discord.gg/dfYAWVMaCW">
-  <img src="https://img.shields.io/discord/1013411447130308669.svg" alt="Discord Channel">
-</a>
+	<img src="https://github.com/sepandhaghighi/pyrgg/raw/master/otherfile/logo.png" width="450">
+	<h1>PyRGG: Python Random Graph Generator</h1>
+	<a href="http://www.shaghighi.ir/pyrgg">
+		<img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg?label=website">
+	</a>
+	<a href="https://badge.fury.io/py/pyrgg">
+		<img src="https://badge.fury.io/py/pyrgg.svg" alt="PyPI version" height="18">
+	</a>
+	<a href="https://anaconda.org/sepandhaghighi/pyrgg">
+		<img src="https://anaconda.org/sepandhaghighi/pyrgg/badges/version.svg">
+	</a>
+	<a href="https://codecov.io/gh/sepandhaghighi/pyrgg">
+  		<img src="https://codecov.io/gh/sepandhaghighi/pyrgg/branch/master/graph/badge.svg" alt="Codecov">
+	</a>
+	<a href="https://www.python.org/">
+		<img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3">
+	</a>
+	<a href="https://discord.gg/dfYAWVMaCW">
+  		<img src="https://img.shields.io/discord/1013411447130308669.svg" alt="Discord Channel">
+	</a>
 </div>	
 
-----------
 ## Table of Contents					
    * [Overview](https://github.com/sepandhaghighi/pyrgg#overview)
    * [Installation](https://github.com/sepandhaghighi/pyrgg#installation)
    * [Usage](https://github.com/sepandhaghighi/pyrgg#usage)
    * [Supported Formats](https://github.com/sepandhaghighi/pyrgg#supported-formats)
    * [Example of Usage](https://github.com/sepandhaghighi/pyrgg#example-of-usage)
    * [Similar Works](https://github.com/sepandhaghighi/pyrgg#similar-works)
    * [Issues & Bug Reports](https://github.com/sepandhaghighi/pyrgg#issues--bug-reports)
-   * [Dependencies](https://github.com/sepandhaghighi/pyrgg#dependencies)
    * [Contribution](https://github.com/sepandhaghighi/pyrgg/blob/master/.github/CONTRIBUTING.md)
    * [References](https://github.com/sepandhaghighi/pyrgg#references)
    * [Citing](https://github.com/sepandhaghighi/pyrgg#citing)
    * [Authors](https://github.com/sepandhaghighi/pyrgg/blob/master/AUTHORS.md)
    * [License](https://github.com/sepandhaghighi/pyrgg/blob/master/LICENSE)
    * [Show Your Support](https://github.com/sepandhaghighi/pyrgg#show-your-support)
    * [Todo](https://github.com/sepandhaghighi/pyrgg/blob/master/TODO.md)
@@ -124,32 +125,31 @@
 		<td align="center"><a href="https://www.codefactor.io/repository/github/sepandhaghighi/pyrgg"><img src="https://www.codefactor.io/repository/github/sepandhaghighi/pyrgg/badge" alt="CodeFactor" /></a></td>	
 	</tr>
 </table>
 
 
 ## Installation		
 
-### Source Code
-- Download [Version 1.3](https://github.com/sepandhaghighi/pyrgg/archive/v1.3.zip) or [Latest Source ](https://github.com/sepandhaghighi/pyrgg/archive/dev.zip)
-- `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
-- `python3 setup.py install` or `python setup.py install` (Need root access)				
-
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install pyrgg==1.3` or `pip3 install pyrgg==1.3` (Need root access)							
+- `pip install pyrgg==1.4` (Need root access)							
+
+### Source Code
+- Download [Version 1.4](https://github.com/sepandhaghighi/pyrgg/archive/v1.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/pyrgg/archive/dev.zip)
+- `pip install .` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io)
 - `conda install -c sepandhaghighi pyrgg` (Need root access)	
 
 ### Exe Version (Only Windows)
-- Download [Exe-Version 1.3](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.3/PYRGG-1.3.exe)
-- Run `PYRGG-1.3.exe`
+- Download [Exe-Version 1.4](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.4/PYRGG-1.4.exe)
+- Run `PYRGG-1.4.exe`
 
 ### System Requirements
 Pyrgg will likely run on a modern dual core PC. Typical configuration is:
 
 - Dual Core CPU (2.0 Ghz+)
 - 4GB of RAM
 
@@ -510,27 +510,14 @@
 
 You can also join our discord server			
 
 <a href="https://discord.gg/dfYAWVMaCW">
   <img src="https://img.shields.io/discord/1013411447130308669.svg?style=for-the-badge" alt="Discord Channel">
 </a>
 
-## Dependencies
-
-<table>
-	<tr> 
-		<td align="center">master</td>	
-		<td align="center">dev</td>	
-	</tr>
-	<tr>
-		<td align="center"><a href="https://requires.io/github/sepandhaghighi/pyrgg/requirements/?branch=master"><img src="https://requires.io/github/sepandhaghighi/pyrgg/requirements.svg?branch=master" alt="Requirements Status" /></a></td>
-		<td align="center"><a href="https://requires.io/github/sepandhaghighi/pyrgg/requirements/?branch=dev"><img src="https://requires.io/github/sepandhaghighi/pyrgg/requirements.svg?branch=dev" alt="Requirements Status" /></a></td>
-	</tr>
-</table>
-
 
 ## Citing
 
 If you use pyrgg in your research, please cite the [JOSS paper](http://joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg JOSS Paper") ;-)
 
 <pre>
 @article{Haghighi2017,
@@ -583,14 +570,17 @@
 <blockquote>10- Skiena, Steven S. The algorithm design manual. Springer International Publishing, 2020. </blockquote>
 
 <blockquote>11- Chakrabarti, Deepayan, Yiping Zhan, and Christos Faloutsos. "R-MAT: A recursive model for graph mining." Proceedings of the 2004 SIAM International Conference on Data Mining. Society for Industrial and Applied Mathematics, 2004. </blockquote>
 
 <blockquote>12- Zhong, Jianlong, and Bingsheng He. "An overview of medusa: simplified graph processing on gpus." ACM SIGPLAN Notices 47.8 (2012): 283-284.</blockquote>
 
 <blockquote>13- Ellson, John, et al. "Graphviz and dynagraph—static and dynamic graph drawing tools." Graph drawing software. Springer, Berlin, Heidelberg, 2004. 127-148.</blockquote>
+
+
+* Logo designed by [Zahra Mobasher](https://www.instagram.com/littleblackoyster)	
 					
  
 ## Show Your Support
 								
 <h3>Star This Repo</h3>					
 
 Give a ⭐️ if this project helped you!
@@ -618,22 +608,35 @@
 <h4>Stellar</h4>		
 GALPOLPISRHIYHLQER2TLJRGUSZH52RYDK6C3HIU4PSMNAV65Q36EGNL
 <h4>Zilliqa</h4>
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 <h4>Coffeete</h4>
 <a href="http://www.coffeete.ir/opensource">
 <img src="http://www.coffeete.ir/images/buttons/lemonchiffon.png" style="width:260px;" />
-</a>	
+</a>
+
+
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.4] - 2023-07-06
+### Added
+- `check_for_config` function
+- `load_config` function
+- `save_config` function
+### Changed
+- `README.md` modified
+- Logo changed
+- `codecov` removed from `dev-requirements.txt`
+- Test system modified
+- Error messages updated
 ## [1.3] - 2022-11-30
 ### Added
 - Graphviz(DOT) format
 ### Changed
 - [asciinema](https://asciinema.org) instruction video updated
 - Test system modified
 - `README.md` modified
@@ -779,15 +782,16 @@
 
 ## [0.1] - 2017-08-19
 ### Added
 - DIMACS format
 - JSON format
 - README
 
-[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.3...dev
+[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.4...dev
+[1.4]: https://github.com/sepandhaghighi/pyrgg/compare/v1.3...v1.4
 [1.3]: https://github.com/sepandhaghighi/pyrgg/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/pyrgg/compare/v1.1...v1.2
 [1.1]: https://github.com/sepandhaghighi/pyrgg/compare/v1.0...v1.1
 [1.0]: https://github.com/sepandhaghighi/pyrgg/compare/v0.9...v1.0
 [0.9]: https://github.com/sepandhaghighi/pyrgg/compare/v0.8...v0.9
 [0.8]: https://github.com/sepandhaghighi/pyrgg/compare/v0.7...v0.8
 [0.7]: https://github.com/sepandhaghighi/pyrgg/compare/v0.6...v0.7
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pyrgg Version: 1.3 Summary: Python Random Graph
+Metadata-Version: 2.1 Name: pyrgg Version: 1.4 Summary: Python Random Graph
 Generator Home-page: https://github.com/sepandhaghighi/pyrgg Download-URL:
-https://github.com/sepandhaghighi/pyrgg/tarball/v1.3 Author: PyRGG Development
+https://github.com/sepandhaghighi/pyrgg/tarball/v1.4 Author: PyRGG Development
 Team Author-email: info@pyrgg.ir License: MIT Project-URL: Webpage, https://
 www.pyrgg.ir Project-URL: Source, https://github.com/sepandhaghighi/pyrgg
 Keywords: random graph python3 python generator graph-process generator DIMACS
 JSON YAML Pickle CSV TSV WEL ASP TGF UCINET Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -19,73 +19,68 @@
 Analysis Classifier: Topic :: Education Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Human Machine
 Interfaces Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.md
-            [http://www.shaghighi.ir/pyrgg/images/pyrgg-logo.png]
-===============================================================================
-                     ****** Random Graph Generator ******
+    [https://github.com/sepandhaghighi/pyrgg/raw/master/otherfile/logo.png]
+              ****** PyRGG: Python Random Graph Generator ******
             [https://img.shields.io/website-up-down-green-red/http/
       shields.io.svg?label=website] [PyPI_version] [https://anaconda.org/
    sepandhaghighi/pyrgg/badges/version.svg] [Codecov] [built_with_Python3]
                                [Discord_Channel]
- ---------- ## Table of Contents * [Overview](https://github.com/
-sepandhaghighi/pyrgg#overview) * [Installation](https://github.com/
-sepandhaghighi/pyrgg#installation) * [Usage](https://github.com/sepandhaghighi/
-pyrgg#usage) * [Supported Formats](https://github.com/sepandhaghighi/
-pyrgg#supported-formats) * [Example of Usage](https://github.com/
-sepandhaghighi/pyrgg#example-of-usage) * [Similar Works](https://github.com/
-sepandhaghighi/pyrgg#similar-works) * [Issues & Bug Reports](https://
-github.com/sepandhaghighi/pyrgg#issues--bug-reports) * [Dependencies](https://
-github.com/sepandhaghighi/pyrgg#dependencies) * [Contribution](https://
-github.com/sepandhaghighi/pyrgg/blob/master/.github/CONTRIBUTING.md) *
-[References](https://github.com/sepandhaghighi/pyrgg#references) * [Citing]
-(https://github.com/sepandhaghighi/pyrgg#citing) * [Authors](https://
-github.com/sepandhaghighi/pyrgg/blob/master/AUTHORS.md) * [License](https://
-github.com/sepandhaghighi/pyrgg/blob/master/LICENSE) * [Show Your Support]
-(https://github.com/sepandhaghighi/pyrgg#show-your-support) * [Todo](https://
-github.com/sepandhaghighi/pyrgg/blob/master/TODO.md) * [Changelog](https://
-github.com/sepandhaghighi/pyrgg/blob/master/CHANGELOG.md) * [Code of Conduct]
-(https://github.com/sepandhaghighi/pyrgg/blob/master/.github/
-CODE_OF_CONDUCT.md) ## Overview Pyrgg is an easy-to-use synthetic random graph
-generator written in Python which supports various graph file formats including
-DIMACS_.gr files. Pyrgg has the ability to generate graphs of different sizes
-and is designed to provide input files for broad range of graph-based research
-applications, including but not limited to testing, benchmarking and
-performance-analysis of graph processing frameworks. Pyrgg target audiences are
-computer scientists who study graph algorithms and graph processing frameworks.
+ ## Table of Contents * [Overview](https://github.com/sepandhaghighi/
+pyrgg#overview) * [Installation](https://github.com/sepandhaghighi/
+pyrgg#installation) * [Usage](https://github.com/sepandhaghighi/pyrgg#usage) *
+[Supported Formats](https://github.com/sepandhaghighi/pyrgg#supported-formats)
+* [Example of Usage](https://github.com/sepandhaghighi/pyrgg#example-of-usage)
+* [Similar Works](https://github.com/sepandhaghighi/pyrgg#similar-works) *
+[Issues & Bug Reports](https://github.com/sepandhaghighi/pyrgg#issues--bug-
+reports) * [Contribution](https://github.com/sepandhaghighi/pyrgg/blob/
+master/.github/CONTRIBUTING.md) * [References](https://github.com/
+sepandhaghighi/pyrgg#references) * [Citing](https://github.com/sepandhaghighi/
+pyrgg#citing) * [Authors](https://github.com/sepandhaghighi/pyrgg/blob/master/
+AUTHORS.md) * [License](https://github.com/sepandhaghighi/pyrgg/blob/master/
+LICENSE) * [Show Your Support](https://github.com/sepandhaghighi/pyrgg#show-
+your-support) * [Todo](https://github.com/sepandhaghighi/pyrgg/blob/master/
+TODO.md) * [Changelog](https://github.com/sepandhaghighi/pyrgg/blob/master/
+CHANGELOG.md) * [Code of Conduct](https://github.com/sepandhaghighi/pyrgg/blob/
+master/.github/CODE_OF_CONDUCT.md) ## Overview Pyrgg is an easy-to-use
+synthetic random graph generator written in Python which supports various graph
+file formats including DIMACS_.gr files. Pyrgg has the ability to generate
+graphs of different sizes and is designed to provide input files for broad
+range of graph-based research applications, including but not limited to
+testing, benchmarking and performance-analysis of graph processing frameworks.
+Pyrgg target audiences are computer scientists who study graph algorithms and
+graph processing frameworks.
    Open Hub  [https://www.openhub.net/p/pyrgg/widgets/project_thin_badge.gif]
 PyPI Counter                          [http://pepy.tech/badge/pyrgg]
 Github Stars          [https://img.shields.io/github/stars/sepandhaghighi/
                               pyrgg.svg?style=social&label=Stars]
 Branch                      master                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI          pyrgg/workflows/CI/                 pyrgg/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [codebeat_badge] [CodeFactor]
              11ec048bcd594d84997380b64d2d4add]
-## Installation ### Source Code - Download [Version 1.3](https://github.com/
-sepandhaghighi/pyrgg/archive/v1.3.zip) or [Latest Source ](https://github.com/
-sepandhaghighi/pyrgg/archive/dev.zip) - `pip install -r requirements.txt` or
-`pip3 install -r requirements.txt` (Need root access) - `python3 setup.py
-install` or `python setup.py install` (Need root access) ### PyPI - Check
-[Python Packaging User Guide](https://packaging.python.org/installing/) - `pip
-install pyrgg==1.3` or `pip3 install pyrgg==1.3` (Need root access) ### Conda -
-Check [Conda Managing Package](https://conda.io) - `conda install -
-c sepandhaghighi pyrgg` (Need root access) ### Exe Version (Only Windows) -
-Download [Exe-Version 1.3](https://github.com/sepandhaghighi/pyrgg/releases/
-download/v1.3/PYRGG-1.3.exe) - Run `PYRGG-1.3.exe` ### System Requirements
-Pyrgg will likely run on a modern dual core PC. Typical configuration is: -
-Dual Core CPU (2.0 Ghz+) - 4GB of RAM Note that it may run on lower end
-equipment though good performance is not guaranteed. ## Usage - Open `CMD`
-(Windows) or `Terminal` (UNIX) - Run `pyrgg` or `python -m pyrgg` (or run
-`PYRGG.exe`) - Enter data
+## Installation ### PyPI - Check [Python Packaging User Guide](https://
+packaging.python.org/installing/) - `pip install pyrgg==1.4` (Need root access)
+### Source Code - Download [Version 1.4](https://github.com/sepandhaghighi/
+pyrgg/archive/v1.4.zip) or [Latest Source ](https://github.com/sepandhaghighi/
+pyrgg/archive/dev.zip) - `pip install .` (Need root access) ### Conda - Check
+[Conda Managing Package](https://conda.io) - `conda install -c sepandhaghighi
+pyrgg` (Need root access) ### Exe Version (Only Windows) - Download [Exe-
+Version 1.4](https://github.com/sepandhaghighi/pyrgg/releases/download/v1.4/
+PYRGG-1.4.exe) - Run `PYRGG-1.4.exe` ### System Requirements Pyrgg will likely
+run on a modern dual core PC. Typical configuration is: - Dual Core CPU (2.0
+Ghz+) - 4GB of RAM Note that it may run on lower end equipment though good
+performance is not guaranteed. ## Usage - Open `CMD` (Windows) or `Terminal`
+(UNIX) - Run `pyrgg` or `python -m pyrgg` (or run `PYRGG.exe`) - Enter data
                      [https://asciinema.org/a/539844.svg]
 ## Supported Formats - [DIMACS(.gr)](http://www.diag.uniroma1.it/challenge9/
 format.shtml) ``` p sp   a    . . . a    ``` * [Sample 1](https://
 www.dropbox.com/s/i80tnwuuv4iyqet/100.gr.gz?dl=0) (100 Vertices , 3KB) *
 [Sample 2](https://www.dropbox.com/s/lqk42pwu7o4xauv/1000.gr.gz?dl=0) (1000
 Vertices , 13KB) * [Sample 3](https://www.dropbox.com/s/93dp8cjs6lnu83u/
 1000000.gr.gz?dl=0) (1000000 Vertices , 7MB) * [Sample 4](https://
@@ -174,20 +169,17 @@
 github.com/prathasah/random-modular-network-generator) Generates random graphs
 with tunable strength of community structure - [randomGraph](https://
 github.com/sdghafouri/randomGraph) very simple random graph generator in MATLAB
 - [Graph1](https://github.com/Saptaparni/Graph1) Random Graph Generator with
 Max capacity paths (C++) ## Issues & Bug Reports Just fill an issue and
 describe it. We'll check it ASAP! or send an email to [info@pyrgg.ir](mailto:
 info@pyrgg.ir "info@pyrgg.ir"). You can also join our discord server [Discord
-Channel] ## Dependencies
-           master                  dev
-[Requirements_Status] [Requirements_Status]
-## Citing If you use pyrgg in your research, please cite the [JOSS paper](http:
-//joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg JOSS Paper") ;-
-)
+Channel] ## Citing If you use pyrgg in your research, please cite the [JOSS
+paper](http://joss.theoj.org/papers/da33f691984d9a35f66ff93a391bbc26 "Pyrgg
+JOSS Paper") ;-)
 @article{Haghighi2017,
   doi = {10.21105/joss.00331},
   url = {https://doi.org/10.21105/joss.00331},
   year  = {2017},
   month = {sep},
   publisher = {The Open Journal},
   volume = {2},
@@ -224,15 +216,16 @@
      and Applied Mathematics, 2004.
      12- Zhong, Jianlong, and Bingsheng He. "An overview of medusa:
      simplified graph processing on gpus." ACM SIGPLAN Notices 47.8
      (2012): 283-284.
      13- Ellson, John, et al. "Graphviz and dynagraphâstatic and dynamic
      graph drawing tools." Graph drawing software. Springer, Berlin,
      Heidelberg, 2004. 127-148.
-## Show Your Support
+* Logo designed by [Zahra Mobasher](https://www.instagram.com/
+littleblackoyster) ## Show Your Support
 **** Star This Repo ****
  Give a â­ï¸ if this project helped you!
 **** Donate to Our Project ****
 *** Bitcoin ***
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 *** Ethereum ***
 0xcD4Db18B6664A9662123D4307B074aE968535388
@@ -251,69 +244,73 @@
 *** Dash ***
 Xd3Yn2qZJ7VE8nbKw2fS98aLxR5M6WUU3s
 *** Stellar ***
  GALPOLPISRHIYHLQER2TLJRGUSZH52RYDK6C3HIU4PSMNAV65Q36EGNL
 *** Zilliqa ***
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 *** Coffeete ***
-[http://www.coffeete.ir/images/buttons/lemonchiffon.png]
- # Changelog All notable changes to this project will be documented in this
-file. The format is based on [Keep a Changelog](http://keepachangelog.com/en/
-1.0.0/) and this project adheres to [Semantic Versioning](http://semver.org/
-spec/v2.0.0.html). ## [Unreleased] ## [1.3] - 2022-11-30 ### Added - Graphviz
-(DOT) format ### Changed - [asciinema](https://asciinema.org) instruction video
-updated - Test system modified - `README.md` modified - `Python 3.11` added to
-`test.yml` - CLI mode updated - `dev-requirements.txt` updated - To-do list
-moved to `TODO.md` ## [1.2] - 2022-09-07 ### Added - Anaconda workflow -
-Discord badge ### Changed - Menu optimized - Docstrings modified - `branch_gen`
-function modified - `edge_gen` function modified - `precision` and `min_edge`
-parameters added to `branch_gen` function - `random_edge` parameter removed
-from `branch_gen` function - Test system modified - `AUTHORS.md` updated -
-License updated - `README.md` modified - `Python 3.10` added to `test.yml` ###
-Removed - `sign_gen` function - `random_edge_limits` function ## [1.1] - 2021-
-06-09 ### Added - `requirements-splitter.py` - `is_weighted` function -
-`_write_properties_to_json` function - `PYRGG_TEST_MODE` parameter ### Changed
-- Test system modified - JSON, YAML and Pickle formats value changed from
-`string` to `number` - `properties` section added to JSON, YAML and Pickle
-formats - `_write_to_json` function renamed to `_write_data_to_json` - `logger`
-function modified - `time_convert` function modified - `branch_gen` function
-modified - References updated ## [1.0] - 2021-01-11 ### Added - Number of files
-option ### Changed - All flags type changed to `bool` - Menu optimized - The
-`logger` function enhanced. - Time format in the `logger` changed to `%Y-%m-%d
-%H:%M:%S` - `dl_maker` function modified - `tgf_maker` function modified -
-`gdf_maker` function modified - `run` function modified ## [0.9] - 2020-10-07
-### Added - GEXF format - Float weight support - `tox.ini` ### Changed - Menu
-optimized - `pyrgg.py` renamed to `graph_gen.py` - Other functions moved to
-`functions.py` - Test system modified - `params.py` refactored - `graph_gen.py`
-refactored - `functions.py` refactored - `weight_str_to_number` function
-renamed to `convert_str_to_number` - `branch_gen` function bugs fixed -
-`input_filter` function bug fixed - `gl_maker` function bug fixed -
-`CONTRIBUTING.md` updated - `AUTHORS.md` updated ### Removed - `print_test`
-function - `left_justify` function - `justify` function - `zero_insert`
-function ## [0.8] - 2020-08-19 ### Added - GDF format - GML format ### Changed
-- CLI snapshots updated - `AUTHORS.md` updated ## [0.7] - 2020-08-07 ### Added
-- Graph Line format ### Changed - Menu optimized ## [0.6] - 2020-07-24 ###
-Added - Matrix Market format ### Changed - `json_maker` function optimized -
-`dl_maker` function optimized - `tgf_maker` function optimized - `lp_maker`
-function optimized ## [0.5] - 2020-07-01 ### Added - TSV format - Multigraph
-control ### Changed - `branch_gen` function modified - Website changed to
-[https://www.pyrgg.ir](https://www.pyrgg.ir) ## [0.4] - 2020-06-17 ### Added -
-Self loop control - Github action ### Changed - `appveyor.yml` updated ## [0.3]
-- 2019-11-29 ### Added - `__version__` variable - `CHANGELOG.md` - `dev-
-requirements.txt` - `requirements.txt` - `CODE_OF_CONDUCT.md` -
-`ISSUE_TEMPLATE.md` - `PULL_REQUEST_TEMPLATE.md` - `CONTRIBUTING.md` -
-`version_check.py` - `pyrgg_profile.py` - Unweighted graph - Undirected graph -
-Exe version ### Changed - Test system modified - `README.md` modified -
-Docstrings modified - `get_input` function modified - `edge_gen` function
-modified - Parameters moved to `params.py` ## [0.2] - 2017-09-20 ### Added -
-CSV format - YAML format - Weighted edge list format (WEL) - ASP format -
-Trivial graph format (TGF) - UCINET DL format - Pickle format ## [0.1] - 2017-
-08-19 ### Added - DIMACS format - JSON format - README [Unreleased]: https://
-github.com/sepandhaghighi/pyrgg/compare/v1.3...dev [1.3]: https://github.com/
-sepandhaghighi/pyrgg/compare/v1.2...v1.3 [1.2]: https://github.com/
+[http://www.coffeete.ir/images/buttons/lemonchiffon.png] # Changelog All
+notable changes to this project will be documented in this file. The format is
+based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
+project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
+## [Unreleased] ## [1.4] - 2023-07-06 ### Added - `check_for_config` function -
+`load_config` function - `save_config` function ### Changed - `README.md`
+modified - Logo changed - `codecov` removed from `dev-requirements.txt` - Test
+system modified - Error messages updated ## [1.3] - 2022-11-30 ### Added -
+Graphviz(DOT) format ### Changed - [asciinema](https://asciinema.org)
+instruction video updated - Test system modified - `README.md` modified -
+`Python 3.11` added to `test.yml` - CLI mode updated - `dev-requirements.txt`
+updated - To-do list moved to `TODO.md` ## [1.2] - 2022-09-07 ### Added -
+Anaconda workflow - Discord badge ### Changed - Menu optimized - Docstrings
+modified - `branch_gen` function modified - `edge_gen` function modified -
+`precision` and `min_edge` parameters added to `branch_gen` function -
+`random_edge` parameter removed from `branch_gen` function - Test system
+modified - `AUTHORS.md` updated - License updated - `README.md` modified -
+`Python 3.10` added to `test.yml` ### Removed - `sign_gen` function -
+`random_edge_limits` function ## [1.1] - 2021-06-09 ### Added - `requirements-
+splitter.py` - `is_weighted` function - `_write_properties_to_json` function -
+`PYRGG_TEST_MODE` parameter ### Changed - Test system modified - JSON, YAML and
+Pickle formats value changed from `string` to `number` - `properties` section
+added to JSON, YAML and Pickle formats - `_write_to_json` function renamed to
+`_write_data_to_json` - `logger` function modified - `time_convert` function
+modified - `branch_gen` function modified - References updated ## [1.0] - 2021-
+01-11 ### Added - Number of files option ### Changed - All flags type changed
+to `bool` - Menu optimized - The `logger` function enhanced. - Time format in
+the `logger` changed to `%Y-%m-%d %H:%M:%S` - `dl_maker` function modified -
+`tgf_maker` function modified - `gdf_maker` function modified - `run` function
+modified ## [0.9] - 2020-10-07 ### Added - GEXF format - Float weight support -
+`tox.ini` ### Changed - Menu optimized - `pyrgg.py` renamed to `graph_gen.py` -
+Other functions moved to `functions.py` - Test system modified - `params.py`
+refactored - `graph_gen.py` refactored - `functions.py` refactored -
+`weight_str_to_number` function renamed to `convert_str_to_number` -
+`branch_gen` function bugs fixed - `input_filter` function bug fixed -
+`gl_maker` function bug fixed - `CONTRIBUTING.md` updated - `AUTHORS.md`
+updated ### Removed - `print_test` function - `left_justify` function -
+`justify` function - `zero_insert` function ## [0.8] - 2020-08-19 ### Added -
+GDF format - GML format ### Changed - CLI snapshots updated - `AUTHORS.md`
+updated ## [0.7] - 2020-08-07 ### Added - Graph Line format ### Changed - Menu
+optimized ## [0.6] - 2020-07-24 ### Added - Matrix Market format ### Changed -
+`json_maker` function optimized - `dl_maker` function optimized - `tgf_maker`
+function optimized - `lp_maker` function optimized ## [0.5] - 2020-07-01 ###
+Added - TSV format - Multigraph control ### Changed - `branch_gen` function
+modified - Website changed to [https://www.pyrgg.ir](https://www.pyrgg.ir) ##
+[0.4] - 2020-06-17 ### Added - Self loop control - Github action ### Changed -
+`appveyor.yml` updated ## [0.3] - 2019-11-29 ### Added - `__version__` variable
+- `CHANGELOG.md` - `dev-requirements.txt` - `requirements.txt` -
+`CODE_OF_CONDUCT.md` - `ISSUE_TEMPLATE.md` - `PULL_REQUEST_TEMPLATE.md` -
+`CONTRIBUTING.md` - `version_check.py` - `pyrgg_profile.py` - Unweighted graph
+- Undirected graph - Exe version ### Changed - Test system modified -
+`README.md` modified - Docstrings modified - `get_input` function modified -
+`edge_gen` function modified - Parameters moved to `params.py` ## [0.2] - 2017-
+09-20 ### Added - CSV format - YAML format - Weighted edge list format (WEL) -
+ASP format - Trivial graph format (TGF) - UCINET DL format - Pickle format ##
+[0.1] - 2017-08-19 ### Added - DIMACS format - JSON format - README
+[Unreleased]: https://github.com/sepandhaghighi/pyrgg/compare/v1.4...dev [1.4]:
+https://github.com/sepandhaghighi/pyrgg/compare/v1.3...v1.4 [1.3]: https://
+github.com/sepandhaghighi/pyrgg/compare/v1.2...v1.3 [1.2]: https://github.com/
 sepandhaghighi/pyrgg/compare/v1.1...v1.2 [1.1]: https://github.com/
 sepandhaghighi/pyrgg/compare/v1.0...v1.1 [1.0]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.9...v1.0 [0.9]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.8...v0.9 [0.8]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.7...v0.8 [0.7]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.6...v0.7 [0.6]: https://github.com/
 sepandhaghighi/pyrgg/compare/v0.5...v0.6 [0.5]: https://github.com/
```

### Comparing `pyrgg-1.3/setup.py` & `pyrgg-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,22 +40,22 @@
     except Exception:
         return PYRGG_DESCRIPTION.replace("\n", " ")
 
 
 setup(
     name='pyrgg',
     packages=['pyrgg'],
-    version='1.3',
+    version='1.4',
     description='Python Random Graph Generator',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='PyRGG Development Team',
     author_email='info@pyrgg.ir',
     url='https://github.com/sepandhaghighi/pyrgg',
-    download_url='https://github.com/sepandhaghighi/pyrgg/tarball/v1.3',
+    download_url='https://github.com/sepandhaghighi/pyrgg/tarball/v1.4',
     keywords='random graph python3 python generator graph-process generator DIMACS JSON YAML Pickle CSV TSV WEL ASP TGF UCINET',
     project_urls={
         'Webpage': 'https://www.pyrgg.ir',
         'Source': 'https://github.com/sepandhaghighi/pyrgg',
     },
     install_requires=get_requires(),
     python_requires='>=3.5',
```

