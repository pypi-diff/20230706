# Comparing `tmp/zipline-cli-0.1.2.tar.gz` & `tmp/zipline-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline-cli-0.1.2.tar", last modified: Mon Jul  3 09:48:47 2023, max compression
+gzip compressed data, was "zipline-cli-0.1.3.tar", last modified: Wed Jul  5 23:12:04 2023, max compression
```

## Comparing `zipline-cli-0.1.2.tar` & `zipline-cli-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:48:47.988037 zipline-cli-0.1.2/
--rw-rw-rw-   0        0        0     3660 2023-07-03 09:48:47.988537 zipline-cli-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2980 2023-07-03 09:38:23.000000 zipline-cli-0.1.2/README.md
--rw-rw-rw-   0        0        0      161 2023-07-03 09:48:47.990038 zipline-cli-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-07-03 09:39:03.000000 zipline-cli-0.1.2/setup.py
--rw-rw-rw-   0        0        0     7003 2023-07-03 09:42:32.000000 zipline-cli-0.1.2/zipline.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:48:47.987536 zipline-cli-0.1.2/zipline_cli.egg-info/
--rw-rw-rw-   0        0        0     3660 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 09:48:47.000000 zipline-cli-0.1.2/zipline_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 23:12:04.231492 zipline-cli-0.1.3/
+-rw-rw-rw-   0        0        0     5049 2023-07-05 23:12:04.231994 zipline-cli-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4333 2023-07-05 23:02:29.000000 zipline-cli-0.1.3/README.md
+-rw-rw-rw-   0        0        0      161 2023-07-05 23:12:04.232494 zipline-cli-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2023-07-05 22:52:43.000000 zipline-cli-0.1.3/setup.py
+-rw-rw-rw-   0        0        0     7903 2023-07-05 23:08:50.000000 zipline-cli-0.1.3/zipline.py
+drwxrwxrwx   0        0        0        0 2023-07-05 23:12:04.230992 zipline-cli-0.1.3/zipline_cli.egg-info/
+-rw-rw-rw-   0        0        0     5049 2023-07-05 23:12:04.000000 zipline-cli-0.1.3/zipline_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-05 23:12:04.000000 zipline-cli-0.1.3/zipline_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 23:12:04.000000 zipline-cli-0.1.3/zipline_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-05 23:12:04.000000 zipline-cli-0.1.3/zipline_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-05 23:12:03.000000 zipline-cli-0.1.3/zipline_cli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-07-05 23:12:04.000000 zipline-cli-0.1.3/zipline_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 23:12:04.000000 zipline-cli-0.1.3/zipline_cli.egg-info/top_level.txt
```

### Comparing `zipline-cli-0.1.2/README.md` & `zipline-cli-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,119 @@
-[![Discord](https://img.shields.io/discord/899171661457293343?color=7289da&label=discord&logo=discord&logoColor=white&style=flat)](https://discord.gg/wXy6m2X8wY)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1eee626c47fa4e6fb8b1ed3efdd3e518)](https://app.codacy.com/gh/cssnr/zipline-cli/dashboard)
-[![PyPI](https://img.shields.io/pypi/v/zipline-cli)](https://pypi.org/project/zipline-cli/)
-[![](https://repository-images.githubusercontent.com/661201286/8dfadbc8-94c0-4eaa-88bd-7ee351859510)](https://zipline.diced.tech/)
+[![Discord](https://img.shields.io/discord/899171661457293343?logo=discord&logoColor=white&label=Discord)](https://discord.gg/wXy6m2X8wY)
+[![PyPI](https://img.shields.io/github/issues-raw/cssnr/zipline-cli?logo=github&logoColor=white&label=Issues)](https://github.com/cssnr/zipline-cli/issues)
+[![Codacy Badge](https://img.shields.io/codacy/grade/1eee626c47fa4e6fb8b1ed3efdd3e518?logo=codacy&logoColor=white&label=Codacy)](https://app.codacy.com/gh/cssnr/zipline-cli/dashboard)
+[![PyPI](https://img.shields.io/pypi/v/zipline-cli?logo=python&logoColor=white&label=PyPi)](https://pypi.org/project/zipline-cli/)
+[![](https://repository-images.githubusercontent.com/661201286/8dfadbc8-94c0-4eaa-88bd-7ee351859510)](https://github.com/cssnr/zipline-cli)
 # Zipline CLI
 
 Python 3 CLI Uploader for Zipline.
+Zipline CLI is currently functional and **Under Active Development**.  
+Please open a [Feature Request](https://github.com/cssnr/zipline-cli/discussions/new?category=feature-requests)
+for new features and submit an [Issue](https://github.com/cssnr/zipline-cli/issues)
+for any bugs you find.
+
+*   Zipline Docs: [https://zipline.diced.tech/](https://zipline.diced.tech/)
+
+## Table of Contents
+
+*   [Quick Start](#quick-start)
+*   [Install](#install)
+*   [CLI Usage](#cli-usage)
+*   [Environment Variables](#environment-variables)
+*   [Python API Reference](#python-api-reference)
+*   [Additional Information](#additional-information)
 
-*   Zipline: [https://zipline.diced.tech/](https://zipline.diced.tech/)
+## Quick Start
 
-This is currently a **WIP** and not complete, but has some useful functions.
+```bash
+python3 -m pip install zipline-cli
+zipline --setup
+```
 
 ## Install
 
 From PyPi using pip:
-```text
+```bash
 python3 -m pip install zipline-cli
 ```
 
 From GitHub using pip:
-```text
+```bash
 python3 -m pip install git+https://github.com/cssnr/zipline-cli.git
 ```
 
+From Source using pip:
+```bash
+git clone https://github.com/cssnr/zipline-cli.git
+python3 -m pip install -e zipline-cli
+```
+
 From Source using setuptools:
-```text
+```bash
 git clone https://github.com/cssnr/zipline-cli.git
 cd zipline-cli
 python3 setup.py install
 ```
 
-Uninstall:
-```text
+### Uninstall
+
+To completely remove from any above install methods:
+```bash
 python3 -m pip uninstall zipline-cli
 ```
 
 ## CLI Usage
 
-You will need a Zipline URL and Token to use the utility.
-
 Setup Zipline URL and Token:
 ```bash
 zipline --setup
 ```
 
 Upload a File:
 ```bash
 zipline test.txt
 ```
 
+Upload Multiple Files:
+```bash
+zipline file1.txt file2.txt
+```
+
 Create Text File from Input
 ```bash
 cat test.txt | zipline 
 ```
 
-Create Text File from Text
+Create Text File from Clipboard
 ```bash
 zipline
-# type or paste contents followed by Ctrl+D (Ctrl+Z on Windows)
+# Paste or Type contents, followed by a newline, then Ctrl+D (Ctrl+Z on Windows)
 ```
 
 ## Environment Variables
 
 Environment Variables are stored in the `.zipline` file in your home directory.
 
-*   Location: `~/.zipline`
+*   Location: `~/.zipline` or `$HOME/.zipline`
 
 | Variable       | Description                                                                 |
 |----------------|-----------------------------------------------------------------------------|
 | ZIPLINE_URL    | URL to your Zipline Instance                                                |
 | ZIPLINE_TOKEN  | Authorization Token from Zipline                                            |
 | ZIPLINE_EMBED  | Set this enable Embed on your uploads                                       |
 | ZIPLINE_EXPIRE | See: https://zipline.diced.tech/docs/guides/upload-options#image-expiration |
 
-You may also override them by exporting the variables in your current environment.
+You may override them by exporting the variables in your current environment
+or using the corresponding command line arguments. See `-h` for more info.
 
-## API Reference
+## Python API Reference
 
-Initialize the class with your Zipline URL. 
-Everything else is a header passed as a kwarg. 
-The API does not yet support environment variables. 
+Initialize the class with your Zipline URL.
+Everything else is a header passed as a kwarg.
+The API does not yet support environment variables.
 
 Zipline Token/Authorization is a header kwarg and can be passed as follows:
 ```python
 from zipline import Zipline
 zipline = Zipline('ZIPLINE_URL', authorization='ZIPLINE_TOKEN')
 ```
 
@@ -93,9 +124,14 @@
 with open('text.txt') as f:
     url = zipline.send_file('test.txt', f)
 print(url)
 ```
 
 ## Additional Information
 
-> If you have more questions, concerns, or comments? 
-> Join our [Discord](https://discord.gg/wXy6m2X8wY) for more information...
+Still have questions, concerns, or comments?
+
+*   [Feature Requests](https://github.com/cssnr/zipline-cli/discussions/categories/feature-requests)
+*   [Helpdesk Q&A](https://github.com/cssnr/zipline-cli/discussions/categories/helpdesk-q-a)
+*   [Discord](https://discord.gg/wXy6m2X8wY)
+
+> Zipline Guide: Hit That Fresh Nar Nar: [youtube.com/watch?v=bJHYo2aGWgE](https://www.youtube.com/watch?v=bJHYo2aGWgE)
```

### Comparing `zipline-cli-0.1.2/setup.py` & `zipline-cli-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setup(
+    version='0.1.3',
     name='zipline-cli',
-    version='0.1.2',
     description='Python 3 CLI for Zipline',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/cssnr/zipline-cli',
     author='Shane',
     author_email='shane@sapps.me',
     py_modules=['zipline'],
```

### Comparing `zipline-cli-0.1.2/zipline.py` & `zipline-cli-0.1.3/zipline.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,54 +8,93 @@
 import sys
 from decouple import config
 from dotenv import find_dotenv, load_dotenv
 from pathlib import Path
 from typing import Any, Dict, List, Optional, TextIO
 
 
+class ZipURL(object):
+    """
+    Zipline URL Object
+    :param file_url: str: Zipline File Display URL
+    """
+
+    __slots__ = ['url', 'raw']
+
+    def __init__(self, file_url: str):
+        self.url: str = file_url
+        self.raw: str = self._get_raw(file_url)
+
+    def __repr__(self):
+        return f'<url={self.url} raw={self.raw}>'
+
+    def __str__(self):
+        return self.url
+
+    @staticmethod
+    def _get_raw(url: str) -> str:
+        try:
+            s = url.split('/', 4)
+            return f"{s[0]}//{s[2]}/r/{s[4]}"
+        except Exception:
+            return ''
+
+
 class Zipline(object):
     """
     Zipline Python API
-    :param url: str: Zipline URL
+    :param base_url: str: Zipline URL
     :param kwargs: Zipline Headers
     """
     allowed_headers = ['format', 'image_compression_percent', 'expires_at',
                        'password', 'zws', 'embed', 'max_views', 'uploadtext',
                        'authorization', 'no_json', 'x_zipline_filename',
                        'original_name', 'override_domain']
 
-    def __init__(self, zipline_url: str, **kwargs):
-        self.zipline_url: str = zipline_url.rstrip('/')
-        self.headers: Dict[str, str] = {}
+    def __init__(self, base_url: str, **kwargs):
+        self.base_url: str = base_url.rstrip('/')
+        self._headers: Dict[str, str] = {}
         for header, value in kwargs.items():
             if header.lower() not in self.allowed_headers:
                 continue
             if value is None:
                 continue
             key = header.replace('_', '-').title()
-            self.headers[key] = str(value)
+            self._headers[key] = str(value)
 
     def send_file(self, file_name: str, file_object: TextIO,
-                  overrides: Optional[dict] = None) -> str:
+                  overrides: Optional[dict] = None) -> ZipURL:
         """
         Send File to Zipline
         :param file_name: str: Name of File for files tuple
         :param file_object: TextIO: File to Upload
         :param overrides: dict: Header Overrides
         :return: str: File URL
         """
-        url = self.zipline_url + '/api/upload'
+        url = self.base_url + '/api/upload'
         files = {'file': (file_name, file_object)}
-        headers = self.headers | overrides if overrides else self.headers
+        headers = self._headers | overrides if overrides else self._headers
         r = requests.post(url, headers=headers, files=files)
         r.raise_for_status()
-        return r.json()['files'][0]
+        return ZipURL(r.json()['files'][0])
         # return f'https://example.com/dummy/{file_name}'
 
 
+def format_output(filename: str, url: ZipURL) -> str:
+    """
+    Format URL Output
+    :param filename: str: Original or File Name
+    :param url: ZipURL: ZipURL to Format
+    :return: str: Formatted Output
+    """
+    if url.raw:
+        return f'{filename}\n{url}\n{url.raw}'
+    return f'{filename}\n{url}'
+
+
 def gen_rand(length: Optional[int] = 4) -> str:
     """
     Generate Random Streng at Given length
     :param length: int: Length of Random String
     :return: str: Random String
     """
     length: int = length if not length < 0 else 4
@@ -149,30 +188,30 @@
 
     zipline = Zipline(args.url, **vars(args))
 
     if not args.files:
         content: str = sys.stdin.read().rstrip('\n') + '\n'
         text_f: TextIO = io.StringIO(content)
         name = f'{gen_rand(8)}.txt'
-        url: str = zipline.send_file(name, text_f)
-        print(f'{name} -> {url}')
+        url: ZipURL = zipline.send_file(name, text_f)
+        print(format_output(name, url))
         sys.exit(0)
 
     exit_code = 1
-    for filename in args.files:
-        if not os.path.isfile(filename):
-            print(f'Warning: File Not Found: {filename}')
+    for name in args.files:
+        if not os.path.isfile(name):
+            print(f'Warning: File Not Found: {name}')
             continue
-        with open(filename) as f:
+        with open(name) as f:
             # name, ext = os.path.splitext(os.path.basename(filename))
             # ext = f'.{ext}' if ext else ''
             # name = f'{name}-{gen_rand(8)}{ext}'
             # url: str = zipline.send_file(name, f)
-            url: str = zipline.send_file(filename, f)
-            print(f'{filename} -> {url}')
+            url: ZipURL = zipline.send_file(name, f)
+            print(format_output(name, url))
             exit_code = 0
     sys.exit(exit_code)
 
 
 if __name__ == '__main__':
     try:
         main()
```

