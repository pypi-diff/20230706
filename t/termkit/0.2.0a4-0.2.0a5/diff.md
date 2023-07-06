# Comparing `tmp/termkit-0.2.0a4.tar.gz` & `tmp/termkit-0.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termkit-0.2.0a4.tar", max compression
+gzip compressed data, was "termkit-0.2.0a5.tar", max compression
```

## Comparing `termkit-0.2.0a4.tar` & `termkit-0.2.0a5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a4/LICENSE
--rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a4/README.md
--rw-r--r--   0        0        0      697 2023-07-06 08:56:45.316124 termkit-0.2.0a4/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-21 20:43:42.356239 termkit-0.2.0a4/termkit/__init__.py
--rw-r--r--   0        0        0     6550 2023-06-27 15:28:33.270769 termkit-0.2.0a4/termkit/arguments.py
--rw-r--r--   0        0        0    14140 2023-07-06 08:56:36.318901 termkit-0.2.0a4/termkit/components.py
--rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a4/termkit/exceptions.py
--rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a4/termkit/formatters.py
--rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a4/termkit/groups.py
--rw-r--r--   0        0        0     1291 2023-06-21 20:43:42.316239 termkit-0.2.0a4/termkit/helpers.py
--rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a4/termkit/tests.py
--rw-r--r--   0        0        0     3879 1970-01-01 00:00:00.000000 termkit-0.2.0a4/setup.py
--rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 termkit-0.2.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a5/LICENSE
+-rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a5/README.md
+-rw-r--r--   0        0        0      697 2023-07-06 08:58:02.049149 termkit-0.2.0a5/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-21 20:43:42.356239 termkit-0.2.0a5/termkit/__init__.py
+-rw-r--r--   0        0        0     6550 2023-06-27 15:28:33.270769 termkit-0.2.0a5/termkit/arguments.py
+-rw-r--r--   0        0        0    14216 2023-07-06 08:57:50.672679 termkit-0.2.0a5/termkit/components.py
+-rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a5/termkit/exceptions.py
+-rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a5/termkit/formatters.py
+-rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a5/termkit/groups.py
+-rw-r--r--   0        0        0     1291 2023-06-21 20:43:42.316239 termkit-0.2.0a5/termkit/helpers.py
+-rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a5/termkit/tests.py
+-rw-r--r--   0        0        0     3879 1970-01-01 00:00:00.000000 termkit-0.2.0a5/setup.py
+-rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 termkit-0.2.0a5/PKG-INFO
```

### Comparing `termkit-0.2.0a4/LICENSE` & `termkit-0.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/README.md` & `termkit-0.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/pyproject.toml` & `termkit-0.2.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "termkit"
-version = "0.2.0a4"
+version = "0.2.0a5"
 description = "Command Line Tools with ease"
 authors = ["Thomas Mahé <contact@tmahe.dev>"]
 readme = "README.md"
 
 #[tool.poetry.scripts]
 #termkit = 'termkit.app:entry_point'
```

### Comparing `termkit-0.2.0a4/termkit/arguments.py` & `termkit-0.2.0a5/termkit/arguments.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/termkit/components.py` & `termkit-0.2.0a5/termkit/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
         self.app_name = os.path.basename(sys.argv[0])
         self._files = [
             Path.home().joinpath('.config').joinpath(self.app_name).joinpath("profile.yaml"),
             Path.home().joinpath('.config').joinpath(self.app_name).joinpath("profile.yml"),
             Path.cwd().joinpath(f'.{self.app_name}.yaml'),
             Path.cwd().joinpath(f'.{self.app_name}.yml'),
         ]
+
+        for e in self._files:
+            print("PROFILE: looking in", e)
+
         if content is not None:
             self._content = content
         else:
             logger = logging.getLogger("termkit.components.ProfileResolver")
             self._content = []
             for file in self._files:
                 if os.path.exists(file):
```

### Comparing `termkit-0.2.0a4/termkit/exceptions.py` & `termkit-0.2.0a5/termkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/termkit/formatters.py` & `termkit-0.2.0a5/termkit/formatters.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/termkit/groups.py` & `termkit-0.2.0a5/termkit/groups.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/termkit/helpers.py` & `termkit-0.2.0a5/termkit/helpers.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/termkit/tests.py` & `termkit-0.2.0a5/termkit/tests.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a4/setup.py` & `termkit-0.2.0a5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'termkit',
-    'version': '0.2.0a4',
+    'version': '0.2.0a5',
     'description': 'Command Line Tools with ease',
     'long_description': '<p align="center">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner.png#gh-dark-mode-only" width="450">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner_light.png#gh-light-mode-only" width="450">\n</p>\n<div align="center">\n  <b><i>Command Line Tools with... ease.</i></b>\n<hr>\n\n[![Tests](https://github.com/thmahe/termkit/actions/workflows/tests.yml/badge.svg)](https://github.com/thmahe/termkit/actions/workflows/tests.yml)\n[![codecov](https://codecov.io/github/thmahe/termkit/branch/master/graph/badge.svg?token=o7UVrOsoq4)](https://codecov.io/github/thmahe/termkit)\n![PyPI](https://img.shields.io/pypi/v/termkit)\n![Platforms](https://img.shields.io/badge/platforms-Linux%20%7C%20MacOS%20%7C%20Windows-lightgrey)\n\n</div>\n\n## Table of Contents\n\n- [Introduction](#introduction)\n- [Features](#features)\n- [Requirement](#requirement)\n- [Installation](#installation)\n- [Examples](#examples)\n- [Feedback](#feedback)\n- [Acknowledgments](#acknowledgments)\n\n## Introduction\n\nTermkit is a framework for building command line interface applications using functions \nand type hints [[PEP 484]](https://peps.python.org/pep-0484/). \n**Solely written using [Python Standard Library](https://docs.python.org/3/library/)** and will always be to ensure\nminimal dependency footprint within your project.\n\nIn few words, Termkit is designed to be the foundation of serious CLI tools.\n\n## Features\n\nA few of the things you can do with Termkit:\n\n* Build CLI from functional code\n* Create fast prototypes using implicit arguments\n* Helpers populated from docstrings\n* Named profile for pre-populated arguments\n* Autocompletion through [argcomplete](https://pypi.org/project/argcomplete/) module\n* Cross-platforms\n\n## Requirement\n* Python 3.7 or higher\n\n*Yes... that\'s about it !* \n\n### Compatibility matrix\n\n|          OS | Python 3.6 |     Python 3.7     |     Python 3.8     |     Python 3.9     |    Python 3.10     |    Python 3.11     |    Python 3.12    |\n|------------:|:----------:|:------------------:|:------------------:|:------------------:|:------------------:|:------------------:|:-----------------:|\n|   **Linux** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n|   **MacOS** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n| **Windows** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n\n\n## Installation\n\nTermkit is published as a [Python package](https://pypi.org/project/termkit) and can be installed with pip.\n\nOpen up a terminal and install Termkit with:\n```shell\npip install termkit\n```\n\n## Examples\n\n### Greeting application\n\n```python\n# greet.py\nimport termkit\n\ndef greet(name):\n    print(f\'Hello {name} !\')\n\nif __name__ == \'__main__\':\n    termkit.run(greet)\n```\n\n```\n$ python3 ./greet.py Thomas\nHello Thomas !\n```\n\n## Feedback\n\nFeel free to send me feedback by [raising an issue](https://github.com/thmahe/termkit/issues/new).\nFeature requests are always welcome.\n\n',
     'author': 'Thomas Mahé',
     'author_email': 'contact@tmahe.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `termkit-0.2.0a4/PKG-INFO` & `termkit-0.2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termkit
-Version: 0.2.0a4
+Version: 0.2.0a5
 Summary: Command Line Tools with ease
 Author: Thomas Mahé
 Author-email: contact@tmahe.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

