# Comparing `tmp/pyvipe-0.1.3.tar.gz` & `tmp/pyvipe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvipe-0.1.3.tar", last modified: Sat Jun 24 21:58:03 2023, max compression
+gzip compressed data, was "pyvipe-0.2.0.tar", last modified: Thu Jul  6 14:03:07 2023, max compression
```

## Comparing `pyvipe-0.1.3.tar` & `pyvipe-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.029747 pyvipe-0.1.3/
--rw-r--r--   0 constantinhong   (501) staff       (20)    17987 2023-06-23 18:49:03.000000 pyvipe-0.1.3/LICENSE
--rw-r--r--   0 constantinhong   (501) staff       (20)    22751 2023-06-24 21:58:03.029345 pyvipe-0.1.3/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      955 2023-06-24 20:24:36.000000 pyvipe-0.1.3/README.md
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.021132 pyvipe-0.1.3/completion/
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.024185 pyvipe-0.1.3/completion/bash/
--rw-r--r--   0 constantinhong   (501) staff       (20)      243 2023-06-24 21:19:54.000000 pyvipe-0.1.3/completion/bash/vipe
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.024733 pyvipe-0.1.3/completion/zsh/
--rw-r--r--   0 constantinhong   (501) staff       (20)      310 2023-06-24 21:25:34.000000 pyvipe-0.1.3/completion/zsh/_vipe
--rw-r--r--   0 constantinhong   (501) staff       (20)     1136 2023-06-24 21:54:08.000000 pyvipe-0.1.3/pyproject.toml
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.025905 pyvipe-0.1.3/pyvipe/
--rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-06-23 20:03:21.000000 pyvipe-0.1.3/pyvipe/__init__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)      137 2023-06-23 20:26:37.000000 pyvipe-0.1.3/pyvipe/__main__.py
--rw-r--r--   0 constantinhong   (501) staff       (20)     2556 2023-06-24 21:51:29.000000 pyvipe-0.1.3/pyvipe/pyvipe.py
-drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-06-24 21:58:03.028756 pyvipe-0.1.3/pyvipe.egg-info/
--rw-r--r--   0 constantinhong   (501) staff       (20)    22751 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/PKG-INFO
--rw-r--r--   0 constantinhong   (501) staff       (20)      291 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/SOURCES.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/dependency_links.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       46 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/entry_points.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)        7 2023-06-24 21:58:02.000000 pyvipe-0.1.3/pyvipe.egg-info/top_level.txt
--rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-06-24 21:58:03.029843 pyvipe-0.1.3/setup.cfg
--rw-r--r--   0 constantinhong   (501) staff       (20)     1456 2023-06-24 21:54:17.000000 pyvipe-0.1.3/setup.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.151829 pyvipe-0.2.0/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    17987 2023-06-23 18:49:03.000000 pyvipe-0.2.0/LICENSE
+-rw-r--r--   0 constantinhong   (501) staff       (20)    23767 2023-07-06 14:03:07.151471 pyvipe-0.2.0/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1971 2023-07-06 14:01:53.000000 pyvipe-0.2.0/README.md
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.143688 pyvipe-0.2.0/completion/
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.146060 pyvipe-0.2.0/completion/bash/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      263 2023-07-06 14:01:53.000000 pyvipe-0.2.0/completion/bash/vipe
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.146390 pyvipe-0.2.0/completion/zsh/
+-rw-r--r--   0 constantinhong   (501) staff       (20)      374 2023-07-06 14:01:53.000000 pyvipe-0.2.0/completion/zsh/_vipe
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1136 2023-07-06 14:01:53.000000 pyvipe-0.2.0/pyproject.toml
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.148517 pyvipe-0.2.0/pyvipe/
+-rw-r--r--   0 constantinhong   (501) staff       (20)        0 2023-07-06 12:47:12.000000 pyvipe-0.2.0/pyvipe/__init__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)      137 2023-06-23 20:26:37.000000 pyvipe-0.2.0/pyvipe/__main__.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)     3108 2023-07-06 14:01:53.000000 pyvipe-0.2.0/pyvipe/pyvipe.py
+-rw-r--r--   0 constantinhong   (501) staff       (20)       22 2023-07-06 12:39:52.000000 pyvipe-0.2.0/pyvipe/version.py
+drwxr-xr-x   0 constantinhong   (501) staff       (20)        0 2023-07-06 14:03:07.150923 pyvipe-0.2.0/pyvipe.egg-info/
+-rw-r--r--   0 constantinhong   (501) staff       (20)    23767 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/PKG-INFO
+-rw-r--r--   0 constantinhong   (501) staff       (20)      309 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/SOURCES.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        1 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/dependency_links.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       46 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/entry_points.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)        7 2023-07-06 14:03:07.000000 pyvipe-0.2.0/pyvipe.egg-info/top_level.txt
+-rw-r--r--   0 constantinhong   (501) staff       (20)       38 2023-07-06 14:03:07.151938 pyvipe-0.2.0/setup.cfg
+-rw-r--r--   0 constantinhong   (501) staff       (20)     1456 2023-07-06 14:01:53.000000 pyvipe-0.2.0/setup.py
```

### Comparing `pyvipe-0.1.3/LICENSE` & `pyvipe-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvipe-0.1.3/PKG-INFO` & `pyvipe-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvipe
-Version: 0.1.3
+Version: 0.2.0
 Summary: edit pipe with your editor.
 Home-page: https://github.com/Constantin1489/pyvipe
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
@@ -368,19 +368,22 @@
 
 * [INTRODUCTION](#introduction)
 * [INSTALLATION](#installation)
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [ENVIRONMENT_VARIABLES](#environment-variables)
+* [FAQ](#faq)
+* [CHANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **pyvipe** is a Python port of [vipe](http://joeyh.name/code/moreutils/).
+**pyvipe**'s command is `vipe`
 
 This project is a by-product of [trrc](https://github.com/Constantin1489/trrc) feature development.
 
 ## INSTALLATION
 
 ### pip
 
@@ -394,17 +397,40 @@
 
 ```
 command1 | vipe | command2
 ```
 
 Use `--suffix` to apply file syntax highlighting.
 
+### pyvipe special options
+
+If you edit such a CRLF PIPE but want vipe to print it as a universial newline, then use `--universal-newline`. This option is for a Windows generated text file.
+
 ## Environment Variables
 
-**pyvipe** chooses the editor to use via looking for editors which are `/usr/bin/editor`, `$EDITOR`, `$VISUAL`, in order.
+**pyvipe** chooses the editor to use with the environment variable `$VISUAL`. If it is unset, it uses `$EDITOR`. If both are unset, it uses  `/usr/bin/editor` if it exists. If none of those work, it defaults to vi.
+
+## FAQ
+
+### Editor exited nonzero, aborting.
+
+In general, editor can exit with nonzero when you execute some command for various purposes. e.g preventing git rebase.
+But if you didn't execute the command but the editor exited with nonzero, it may be because
+of wrong user configuration for the editor.
+
+For vi, you can debug it with `EDITOR='vi -u NONE vipe'`
+
+## Changelog
+
+| Version | Note                     | 
+|:--------|:-------------------------|
+| HEAD    | add universal-newline option. support editor variable with option. | 
+| 0.1.3    | fix shell completion. | 
+| 0.1.2    | add suffix option. fix error. | 
+| 0.1.1   | init                     | 
 
 ## CONTRIBUTION
 
 If it doesn't work as original [vipe](http://joeyh.name/code/moreutils/), then it's a bug.
 
 ## Thanks to
```

### Comparing `pyvipe-0.1.3/pyproject.toml` & `pyvipe-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyvipe"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 maintainers = [
     { name="Constantin Hong", email="hongconstantin@gmail.com" },
 ]
 license = {file = "LICENSE"}
```

### Comparing `pyvipe-0.1.3/pyvipe/pyvipe.py` & `pyvipe-0.2.0/pyvipe/pyvipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import subprocess
 import sys
 import tempfile
 import argparse
 
-VERSION_HELP = """pyvipe - 0.1.3
+VERSION_HELP = """pyvipe - 0.2.0
 Copyright (C) 2023 Constantin Hong
 License GPLv2: GNU GPL version 2 <https://gnu.org/licenses/gpl.html>.
 This is free software: you are free to change and redistribute it.
 There is NO WARRANTY, to the extent permitted by law."""
 
 def pyvipe():
     """Run pyvipe program."""
@@ -25,34 +25,44 @@
             '--suffix',
             action='store',
             dest='suffix',
             default=None,
             help='Add suffix to enable syntax highlighting in your editor.',
             )
     parser.add_argument(
+            '--universal-newline',
+            action='store_true',
+            dest='universal_newline',
+            help='Print stdout with a universal newline.',
+            )
+    parser.add_argument(
             '-V', '--version',
             action='version',
             version=VERSION_HELP,
             help='Print a version number and a license of pyvipe.',
             )
 
-    suffix = parser.parse_args(sys.argv[1:]).suffix
+    parsed_arg = parser.parse_args(sys.argv[1:])
+
+    suffix = parsed_arg.suffix
     if suffix:
         suffix = suffix if suffix.startswith('.') else f'.{suffix}'
 
     editor = 'vi'
     if os.access('/usr/bin/editor', os.X_OK):
         editor = '/usr/bin/editor'
 
     if 'EDITOR' in os.environ:
         editor = os.environ['EDITOR']
 
     if 'VISUAL' in os.environ:
         editor = os.environ['VISUAL']
 
+
+    # if there is no PIPE, then open an empty file.
     text = ''
     if sys.stdin.isatty() is False:
         text = sys.stdin.read()
 
     stdin_fd = os.open('/dev/tty', os.O_RDONLY)
     os.dup2(stdin_fd, 0)
     os.close(stdin_fd)
@@ -65,27 +75,32 @@
 
     try:
         with tempfile.NamedTemporaryFile(suffix=suffix) as temporary_file:
             temporary_file.write(text.encode())
             temporary_file.flush()
 
             try:
-                subprocess.check_call([editor, temporary_file.name])
+                subprocess.check_call([*editor.split(), temporary_file.name])
 
             except subprocess.CalledProcessError:
                 print(f'{editor} exited nonzero, aborting', file=sys.stderr)
                 sys.exit(1)
 
             try:
-                with open(temporary_file.name, 'rb') as edited_pipe:
-                    os.write(out, edited_pipe.read())
+                # if option is true, then read CRLF PIPE and return \n stdout.
+                newline = None if parsed_arg.universal_newline else ""
+                with open(temporary_file.name, 'r', newline=newline) as edited_pipe:
+                    byte_edited_pipe = edited_pipe.read().encode('ascii')
+                    os.write(out, byte_edited_pipe)
 
             except PermissionError:
                 print('cannot read tempfile', file=sys.stderr)
                 sys.exit(1)
 
     except PermissionError:
         print('cannot create tempfile', file=sys.stderr)
         sys.exit(1)
 
+    os.close(out)
+
 if __name__ == "__main__":
     pyvipe()
```

### Comparing `pyvipe-0.1.3/pyvipe.egg-info/PKG-INFO` & `pyvipe-0.2.0/pyvipe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvipe
-Version: 0.1.3
+Version: 0.2.0
 Summary: edit pipe with your editor.
 Home-page: https://github.com/Constantin1489/pyvipe
 Author: Constantin Hong
 Author-email: Constantin Hong <hongconstantin@gmail.com>
 Maintainer: Constantin Hong
 Maintainer-email: Constantin Hong <hongconstantin@gmail.com>
 License: 		    GNU GENERAL PUBLIC LICENSE
@@ -368,19 +368,22 @@
 
 * [INTRODUCTION](#introduction)
 * [INSTALLATION](#installation)
     * [PIP](#pip)
     * [MANUAL_INSTALLATION](#manual-installation)
 * [USAGE](#usage)
 * [ENVIRONMENT_VARIABLES](#environment-variables)
+* [FAQ](#faq)
+* [CHANGELOG](#changelog)
 * [CONTRIBUTION](#contribution)
 
 ## INTRODUCTION
 
 **pyvipe** is a Python port of [vipe](http://joeyh.name/code/moreutils/).
+**pyvipe**'s command is `vipe`
 
 This project is a by-product of [trrc](https://github.com/Constantin1489/trrc) feature development.
 
 ## INSTALLATION
 
 ### pip
 
@@ -394,17 +397,40 @@
 
 ```
 command1 | vipe | command2
 ```
 
 Use `--suffix` to apply file syntax highlighting.
 
+### pyvipe special options
+
+If you edit such a CRLF PIPE but want vipe to print it as a universial newline, then use `--universal-newline`. This option is for a Windows generated text file.
+
 ## Environment Variables
 
-**pyvipe** chooses the editor to use via looking for editors which are `/usr/bin/editor`, `$EDITOR`, `$VISUAL`, in order.
+**pyvipe** chooses the editor to use with the environment variable `$VISUAL`. If it is unset, it uses `$EDITOR`. If both are unset, it uses  `/usr/bin/editor` if it exists. If none of those work, it defaults to vi.
+
+## FAQ
+
+### Editor exited nonzero, aborting.
+
+In general, editor can exit with nonzero when you execute some command for various purposes. e.g preventing git rebase.
+But if you didn't execute the command but the editor exited with nonzero, it may be because
+of wrong user configuration for the editor.
+
+For vi, you can debug it with `EDITOR='vi -u NONE vipe'`
+
+## Changelog
+
+| Version | Note                     | 
+|:--------|:-------------------------|
+| HEAD    | add universal-newline option. support editor variable with option. | 
+| 0.1.3    | fix shell completion. | 
+| 0.1.2    | add suffix option. fix error. | 
+| 0.1.1   | init                     | 
 
 ## CONTRIBUTION
 
 If it doesn't work as original [vipe](http://joeyh.name/code/moreutils/), then it's a bug.
 
 ## Thanks to
```

### Comparing `pyvipe-0.1.3/setup.py` & `pyvipe-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 setup(
     name = 'pyvipe',
-    version = '0.1.3',
+    version = '0.2.0',
     description='edit pipe with your editor.',
     author='Constantin Hong',
     author_email='hongconstantin@gmail.com',
     url='https://github.com/Constantin1489/pyvipe',
     maintainer='Constantin Hong',
     maintainer_email='hongconstantin@gmail.com',
     readme = "README.md",
```

