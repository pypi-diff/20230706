# Comparing `tmp/lazy-model-0.0.5.tar.gz` & `tmp/lazy-model-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy-model-0.0.5.tar", max compression
+gzip compressed data, was "lazy-model-0.1.0b0.tar", max compression
```

## Comparing `lazy-model-0.0.5.tar` & `lazy-model-0.1.0b0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0    11351 2022-12-19 10:12:36.332265 lazy-model-0.0.5/LICENSE
--rw-r--r--   0        0        0     1116 2022-12-19 10:12:36.332265 lazy-model-0.0.5/README.md
--rw-r--r--   0        0        0       75 2022-12-19 10:12:36.332265 lazy-model-0.0.5/lazy_model/__init__.py
--rw-r--r--   0        0        0     4030 2022-12-19 10:12:36.332265 lazy-model-0.0.5/lazy_model/main.py
--rw-r--r--   0        0        0      658 2022-12-19 10:12:36.332265 lazy-model-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 lazy-model-0.0.5/setup.py
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 lazy-model-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/LICENSE
+-rw-r--r--   0        0        0     1116 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/README.md
+-rw-r--r--   0        0        0      101 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/lazy_model/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/lazy_model/main.py
+-rw-r--r--   0        0        0       86 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/lazy_model/nao.py
+-rw-r--r--   0        0        0        0 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/lazy_model/parser/__init__.py
+-rw-r--r--   0        0        0     3775 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/lazy_model/parser/new.py
+-rw-r--r--   0        0        0     3974 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/lazy_model/parser/old.py
+-rw-r--r--   0        0        0      660 2023-07-06 02:44:08.939538 lazy-model-0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 lazy-model-0.1.0b0/setup.py
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 lazy-model-0.1.0b0/PKG-INFO
```

### Comparing `lazy-model-0.0.5/LICENSE` & `lazy-model-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy-model-0.0.5/README.md` & `lazy-model-0.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `lazy-model-0.0.5/lazy_model/main.py` & `lazy-model-0.1.0b0/lazy_model/parser/old.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from typing import Any, Optional, Set, Dict
 
 from pydantic import BaseModel, PrivateAttr, parse_obj_as, ValidationError
 
 from pydantic.error_wrappers import ErrorWrapper
 
+from lazy_model.nao import NAO
+
 ROOT_KEY = "__root__"
 object_setattr = object.__setattr__
 
 
-class NotAnObject:
-    def __repr__(self):
-        return "NAO"
-
-
-NAO = NotAnObject()
-
-
 class LazyModel(BaseModel):
     _store: Dict[str, Any] = PrivateAttr(default_factory=dict)
     _lazily_parsed: bool = PrivateAttr(default=False)
 
     @classmethod
     def lazy_parse(
         cls,
```

### Comparing `lazy-model-0.0.5/pyproject.toml` & `lazy-model-0.1.0b0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-model"
-version = "0.0.5"
+version = "0.1.0b0"
 description = ""
 authors = ["Roman Right <roman-right@protonmail.com>"]
 license = "Apache-2.0"
 include = ["LICENSE"]
 readme = "README.md"
 packages = [{include = "lazy_model"}]
```

### Comparing `lazy-model-0.0.5/setup.py` & `lazy-model-0.1.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['lazy_model']
+['lazy_model', 'lazy_model.parser']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.0']
 
 setup_kwargs = {
     'name': 'lazy-model',
-    'version': '0.0.5',
+    'version': '0.1.0b0',
     'description': '',
     'long_description': '# Lazy parsing for Pydantic models\n\nThis library provides a lazy interface for parsing objects from dictionaries. During the parsing, it saves the raw data inside the object and parses each field on demand.\n\n## Install\n\npoetry\n```shell\npoetry add lazy-model\n```\n\npip\n```shell\npip install lazy-model\n```\n\n## Usage\n\n```python\nfrom lazy_model import LazyModel\nfrom pydantic import validator\n\n\nclass Sample(LazyModel):\n    i: int\n    s: str\n\n    @validator("s")\n    def s_upper(cls, v):\n        return v.upper()\n\n\nobj = Sample.lazy_parse({"i": "10", "s": "test"})\n\n# at this point the data is stored in a raw format inside the object\n\nprint(obj.__dict__)\n\n# >>> {\'i\': NAO, \'s\': NAO}\n\n# NAO - Not An Object. It shows that the field was not parsed yet.\n\nprint(obj.s)\n\n# >>> TEST\n\n# Custom validator works during lazy parsing\n\nprint(obj.__dict__)\n\n# >>> {\'i\': NAO, \'s\': \'TEST\'}\n\n# The `s` field  was already parsed by this step\n\nprint(obj.i, type(obj.i))\n\n# >>> 10 <class \'int\'>\n\n# It converted `10` from string to int based on the annotations\n\nprint(obj.__dict__)\n\n# >>> {\'i\': 10, \'s\': \'TEST\'}\n\n# Everything was parsed\n```',
     'author': 'Roman Right',
     'author_email': 'roman-right@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lazy-model-0.0.5/PKG-INFO` & `lazy-model-0.1.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-model
-Version: 0.0.5
+Version: 0.1.0b0
 Summary: 
 License: Apache-2.0
 Author: Roman Right
 Author-email: roman-right@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

