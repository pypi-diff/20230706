# Comparing `tmp/termynal-0.3.1.tar.gz` & `tmp/termynal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.3.1.tar", max compression
+gzip compressed data, was "termynal-0.4.0.tar", max compression
```

## Comparing `termynal-0.3.1.tar` & `termynal-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1092 2023-06-21 13:00:32.572570 termynal-0.3.1/LICENSE
--rw-r--r--   0        0        0      725 2023-06-21 13:00:32.576570 termynal-0.3.1/README.md
--rw-r--r--   0        0        0     2390 2023-06-21 13:00:32.576570 termynal-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/__init__.py
--rw-r--r--   0        0        0     2281 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/assets/termynal.js
--rw-r--r--   0        0        0     3355 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-06-21 13:00:32.576570 termynal-0.3.1/termynal/plugin.py
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 termynal-0.3.1/setup.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 termynal-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-06 12:49:35.725065 termynal-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1067 2023-07-06 12:49:35.725065 termynal-0.4.0/README.md
+-rw-r--r--   0        0        0     2388 2023-07-06 12:49:35.725065 termynal-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/__init__.py
+-rw-r--r--   0        0        0     2281 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     4617 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/plugin.py
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 termynal-0.4.0/setup.py
+-rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 termynal-0.4.0/PKG-INFO
```

### Comparing `termynal-0.3.1/LICENSE` & `termynal-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.3.1/README.md` & `termynal-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -57,17 +57,46 @@
 
 ````
 ```console
 # comment
 ```
 ````
 
-`mkdocs` plugin
+### Mkdocs integration
+
+Declare the plugin:
 
 ```yaml
 ...
 plugins:
   - termynal
 ...
 ```
 
+Optionally, pass options to the processor:
+
+```yaml
+[...]
+markdown_extensions:
+  - termynal:
+      prompt_literal_start:
+        - "$ "
+        - "&gt; "
+[...]
+```
+
+This config allows you to use another prompt:
+
+````markdown
+<!-- termynal -->
+
+```
+> pip install termynal
+---> 100%
+Installed
+```
+
+````
+
+## Credits
+
 Thanks [ines](https://github.com/ines/termynal)
```

### Comparing `termynal-0.3.1/pyproject.toml` & `termynal-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.1"
+version = "0.4.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.3.1"
+version = "0.4.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
@@ -68,15 +68,15 @@
 [tool.coverage.run]
 omit = ["tests/*", "**/__main__.py", "**/.venv/*", "**/site-packages/*"]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
-fail_under = 93.8
+fail_under = 90
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 addopts = "--strict-markers --showlocals --verbosity 2"
 log_level = "DEBUG"
 
 [tool.ruff]
```

### Comparing `termynal-0.3.1/termynal/assets/termynal.css` & `termynal-0.4.0/termynal/assets/termynal.css`

 * *Files identical despite different names*

### Comparing `termynal-0.3.1/termynal/assets/termynal.js` & `termynal-0.4.0/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.3.1/termynal/plugin.py` & `termynal-0.4.0/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.3.1/setup.py` & `termynal-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'markdown.extensions': ['termynal = termynal.markdown:TermynalExtension'],
  'mkdocs.plugins': ['termynal = termynal.plugin:TermynalPlugin']}
 
 setup_kwargs = {
     'name': 'termynal',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': '',
-    'long_description': '# Termynal\n\nA lightweight and modern animated terminal window.\nBuilt for [mkdocs](https://www.mkdocs.org/).\n\n## Installation\n\n<!-- termynal -->\n\n```\n$ pip install termynal\n---> 100%\nInstalled\n```\n\n[Example](https://daxartio.github.io/termynal/)\n\n## Usage\n\nUse `<!-- termynal -->` before code block\n\n````\n<!-- termynal -->\n\n```\n// code\n```\n````\n\nor `console` in code block\n\n````\n```console\n// code\n```\n````\n\nprogress, prompt `---> 100%`\n\n````\n```console\n$ show progress\n---> 100%\nDone!\n```\n````\n\ncommand, start with `$`\n\n````\n```console\n$ command\n```\n````\n\ncomment, start with `#`\n\n````\n```console\n# comment\n```\n````\n\n`mkdocs` plugin\n\n```yaml\n...\nplugins:\n  - termynal\n...\n```\n\nThanks [ines](https://github.com/ines/termynal)\n',
+    'long_description': '# Termynal\n\nA lightweight and modern animated terminal window.\nBuilt for [mkdocs](https://www.mkdocs.org/).\n\n## Installation\n\n<!-- termynal -->\n\n```\n$ pip install termynal\n---> 100%\nInstalled\n```\n\n[Example](https://daxartio.github.io/termynal/)\n\n## Usage\n\nUse `<!-- termynal -->` before code block\n\n````\n<!-- termynal -->\n\n```\n// code\n```\n````\n\nor `console` in code block\n\n````\n```console\n// code\n```\n````\n\nprogress, prompt `---> 100%`\n\n````\n```console\n$ show progress\n---> 100%\nDone!\n```\n````\n\ncommand, start with `$`\n\n````\n```console\n$ command\n```\n````\n\ncomment, start with `#`\n\n````\n```console\n# comment\n```\n````\n\n### Mkdocs integration\n\nDeclare the plugin:\n\n```yaml\n...\nplugins:\n  - termynal\n...\n```\n\nOptionally, pass options to the processor:\n\n```yaml\n[...]\nmarkdown_extensions:\n  - termynal:\n      prompt_literal_start:\n        - "$ "\n        - "&gt; "\n[...]\n```\n\nThis config allows you to use another prompt:\n\n````markdown\n<!-- termynal -->\n\n```\n> pip install termynal\n---> 100%\nInstalled\n```\n\n````\n\n## Credits\n\nThanks [ines](https://github.com/ines/termynal)\n',
     'author': 'Danil Akhtarov',
     'author_email': 'daxartio@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/termynal',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `termynal-0.3.1/PKG-INFO` & `termynal-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -77,18 +77,47 @@
 
 ````
 ```console
 # comment
 ```
 ````
 
-`mkdocs` plugin
+### Mkdocs integration
+
+Declare the plugin:
 
 ```yaml
 ...
 plugins:
   - termynal
 ...
 ```
 
+Optionally, pass options to the processor:
+
+```yaml
+[...]
+markdown_extensions:
+  - termynal:
+      prompt_literal_start:
+        - "$ "
+        - "&gt; "
+[...]
+```
+
+This config allows you to use another prompt:
+
+````markdown
+<!-- termynal -->
+
+```
+> pip install termynal
+---> 100%
+Installed
+```
+
+````
+
+## Credits
+
 Thanks [ines](https://github.com/ines/termynal)
```

