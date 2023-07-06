# Comparing `tmp/tooey-0.2.0.tar.gz` & `tmp/tooey-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tooey-0.2.0.tar", last modified: Mon Jul  3 19:02:46 2023, max compression
+gzip compressed data, was "tooey-0.3.0.tar", last modified: Thu Jul  6 21:49:29 2023, max compression
```

## Comparing `tooey-0.2.0.tar` & `tooey-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 19:02:46.000000 tooey-0.2.0/
--rw-r--r--   0 simon      (501) staff       (20)    11357 2023-06-29 07:36:21.000000 tooey-0.2.0/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)     3774 2023-07-03 19:02:46.000000 tooey-0.2.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2859 2023-07-02 19:14:03.000000 tooey-0.2.0/README.md
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-03 19:02:46.000000 tooey-0.2.0/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)     1023 2023-07-03 18:45:40.000000 tooey-0.2.0/setup.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 19:02:46.000000 tooey-0.2.0/tooey/
--rw-r--r--   0 simon      (501) staff       (20)       30 2023-06-29 08:16:41.000000 tooey-0.2.0/tooey/__init__.py
--rwxr-xr-x   0 simon      (501) staff       (20)      787 2023-07-03 18:52:39.000000 tooey-0.2.0/tooey/__version__.py
--rw-r--r--   0 simon      (501) staff       (20)    11636 2023-07-03 18:49:04.000000 tooey-0.2.0/tooey/tooey.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 19:02:46.000000 tooey-0.2.0/tooey.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     3774 2023-07-03 19:02:46.000000 tooey-0.2.0/tooey.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      196 2023-07-03 19:02:46.000000 tooey-0.2.0/tooey.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-03 19:02:46.000000 tooey-0.2.0/tooey.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2023-07-03 19:02:46.000000 tooey-0.2.0/tooey.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 21:49:29.000000 tooey-0.3.0/
+-rw-r--r--   0 simon      (501) staff       (20)    11357 2023-06-29 07:36:21.000000 tooey-0.3.0/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)     3754 2023-07-06 21:49:29.000000 tooey-0.3.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2859 2023-07-02 19:14:03.000000 tooey-0.3.0/README.md
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-06 21:49:29.000000 tooey-0.3.0/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)     1023 2023-07-03 18:45:40.000000 tooey-0.3.0/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey/
+-rw-r--r--   0 simon      (501) staff       (20)       30 2023-06-29 08:16:41.000000 tooey-0.3.0/tooey/__init__.py
+-rwxr-xr-x   0 simon      (501) staff       (20)      787 2023-07-05 19:07:13.000000 tooey-0.3.0/tooey/__version__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13219 2023-07-06 21:23:56.000000 tooey-0.3.0/tooey/tooey.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     3754 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      196 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tooey-0.2.0/LICENSE` & `tooey-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooey-0.2.0/PKG-INFO` & `tooey-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tooey
-Version: 0.2.0
+Version: 0.3.0
 Summary: Automatically turn script arguments into an interactive terminal interface
 Home-page: https://github.com/simonrob/tooey
 Author: Simon Robinson
 Author-email: simon@robinson.ac
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/simonrob/tooey/issues
 Project-URL: Source Code, https://github.com/simonrob/tooey
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Terminals
@@ -88,9 +87,7 @@
 ```console
 $ FORCE_TOOEY=1 python tooey_example.py val1 --named-choices 1 3 | sort
 ```
 
 
 ## License
 [Apache 2.0](https://github.com/simonrob/tooey/blob/main/LICENSE)
-
-
```

### Comparing `tooey-0.2.0/README.md` & `tooey-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tooey-0.2.0/setup.py` & `tooey-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tooey-0.2.0/tooey/__version__.py` & `tooey-0.3.0/tooey/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = 'tooey'
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 __description__ = 'Automatically turn script arguments into an interactive terminal interface'
 __author__ = 'Simon Robinson'
 __author_email__ = 'simon@robinson.ac'
 __url__ = 'https://github.com/simonrob/tooey'
 __copyright__ = 'Copyright (c) 2023 Simon Robinson'
 __license__ = 'Apache 2.0'
 __classifiers__ = [  # https://pypi.org/classifiers/
```

### Comparing `tooey-0.2.0/tooey/tooey.py` & `tooey-0.3.0/tooey/tooey.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 """
 Tooey: Gooey, but for TUIs
 Decorate your argparse function with `@Tooey` to be prompted interactively in the terminal to enter each argument
 """
+
+# TODO: use Rich to make an actual interface with selectable options? Check dependencies; see https://textualise.io
+# TODO: mocking stdout/stderr: https://stackoverflow.com/a/55234595/
+# TODO: add subparser support
+
+
 import argparse
+import contextlib
+import functools
 import os
 import sys
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
 from argparse import (
     ArgumentParser,
 
+    # we ignore these action types currently
     _HelpAction,
     _VersionAction,
+    _SubParsersAction,
 
+    # we support these action types
     _StoreConstAction,
     _StoreTrueAction,
     _StoreFalseAction,
     _AppendConstAction,
     _AppendAction,
     _CountAction,
     _StoreAction
 )
 
 _SEPARATOR = '-' * 80
 _YES_CHOICES = ('y', 'yes')
 _YES_CHOICES_STRING = ' / '.join(_YES_CHOICES)
 
 
-# TODO: use Rich to make an actual interface with selectable options? Check dependencies
-# TODO: Finish adding tests
-# TODO: look at Gooey and Rich for keywords
-# TODO: Use Textualise.io
-
-# TODO: once uploaded, delete version 0.0.0
-
-class Tooey(object):
-    def __init__(self, f):
-        self.f = f
-
-    def __call__(self, *args, **kwargs):
+# noinspection PyPep8Naming
+def Tooey(f=None):
+    @functools.wraps(f)
+    def wrapper(*args, **kwargs):
         ArgumentParser.original_parse_args = ArgumentParser.parse_args
         ArgumentParser.original_error = ArgumentParser.error
         ArgumentParser.original_error_message = None
 
         ArgumentParser.parse_args = parse_args
         ArgumentParser.error = error
 
-        result = self.f(*args, **kwargs)
+        result = f(*args, **kwargs)
 
         ArgumentParser.parse_args = ArgumentParser.original_parse_args
         ArgumentParser.error = ArgumentParser.original_error
 
         del ArgumentParser.original_parse_args
         del ArgumentParser.original_error
         del ArgumentParser.original_error_message
 
         return result
 
+    return wrapper
+
 
 def parse_args(self, args=None, namespace=None):
-    self.add_argument('--ignore-tooey', action='store_true', help=argparse.SUPPRESS)
-    self.add_argument('--force-tooey', action='store_true', help=argparse.SUPPRESS)
+    with contextlib.suppress(argparse.ArgumentError):  # ignore if these have already been defined by the base function
+        self.add_argument('--ignore-tooey', action='store_true', help=argparse.SUPPRESS)
+        self.add_argument('--force-tooey', action='store_true', help=argparse.SUPPRESS)
     parsed_args = self.original_parse_args(args, namespace)
 
+    # handle environment variables and tooey-related arguments - if both are set, do not proceed with Tooey
     ignore_tooey = parsed_args.ignore_tooey or os.environ.get('IGNORE_TOOEY')
     force_tooey = parsed_args.force_tooey or os.environ.get('FORCE_TOOEY')
     if ignore_tooey and force_tooey:
         force_tooey = False
     del parsed_args.__dict__['ignore_tooey']
     del parsed_args.__dict__['force_tooey']
     self._actions = [a for a in self._actions if a.dest not in ('ignore_tooey', 'force_tooey')]
@@ -77,74 +84,91 @@
         return parsed_args
 
     print(_SEPARATOR)
     print('Tooey interactive mode starting - presenting script options')
 
     try:
         # we have to use the parser's internal _actions object because there is no other way to get an action's details
+        # first, save the initial values to check what _was_ provided at runtime, skipping help and version actions
+        # because they don't require input, and doing this step separately to option parsing itself because multiple
+        # options can share the same `dest`, so the original value could have been updated before we get to it
+        initial_values = {}
+        ignored_actions = (_HelpAction, _VersionAction, _SubParsersAction)
         for action in self._actions:
-            if type(action) in (_HelpAction, _VersionAction):
-                continue  # these actions do not request user input
+            action_type = type(action)
+            if action_type not in ignored_actions:
+                initial_values[action.dest] = parsed_args.__dict__[action.dest]
+            elif action_type not in (_HelpAction, _VersionAction):
+                # TODO: we print an error, but don't handle these args at all, so any real argparse errors will be
+                #  suppressed - best to drop back to standard argparse if any of these arguments are found?
+                print('\nTooey warning: action type', action_type.__name__, 'is not currently handled - skipping')
+
+        # then, iterate over the available options, gathering any additions via user input
+        for action in filter(lambda a: type(a) not in ignored_actions, self._actions):
 
             option_string = ', '.join(action.option_strings) if action.option_strings else action.dest
             current_value = parsed_args.__dict__[action.dest]
 
             print()
             print('Argument:', option_string, '(required)' if action.required else '')
             print('Help text:', action.help)
 
-            if current_value not in (action.default, []) and type(action) is not _AppendConstAction:
+            if initial_values[action.dest] not in (action.default, []) and type(action) is not _AppendConstAction:
                 # note: currently all `append_const` actions are shown even if some are provided at runtime
                 # we don't exclude these because the intent may be to provide them multiple times
+                # TODO: check the append const behaviour is still what we want (same for normal append?)
                 print('Skipping interactive mode for argument provided at runtime (value: %s)' % current_value)
                 continue
 
-            new_value = _parse_action(action, current_value)
-
-            if isinstance(parsed_args.__dict__[action.dest], list):  # lists should be extended rather than replaced
-                if new_value:
-                    parsed_args.__dict__[action.dest] = list(set(current_value + new_value))
-            else:
-                parsed_args.__dict__[action.dest] = new_value
-
+            parsed_args.__dict__[action.dest] = _parse_action(action, current_value)
             print('Outcome:', action.dest, 'is `%s`' % parsed_args.__dict__[action.dest])
 
         print('\nTooey interactive mode completed - continuing script')
         print(_SEPARATOR)
 
         return parsed_args
 
     except KeyboardInterrupt:
         print('\n\nTooey interactive mode interrupted - continuing script')
         print(_SEPARATOR)
         if self.original_error_message:
             self.original_error(self.original_error_message)
 
 
+def get_input(prompt='', strip=False):
+    print(prompt, end=' ')
+    response = input()
+    if not response:  # testing can produce an actual `None` where real input would only lead to an empty string
+        response = ''
+    if strip:
+        response = response.strip()
+    if 'unittest' in sys.modules:
+        print(response)
+    return response
+
+
 def _parse_action(action, current_value):
     action_type = type(action)
 
     if action_type in (_StoreConstAction, _StoreTrueAction, _StoreFalseAction):
         # these action types provide a constant value - either user-defined, or True/False
         yes_response = action.const if action_type is _StoreConstAction else not action.default
         if action.required:
             print('Skipping interactive mode for required action - the only possible value is `%s`' % yes_response)
             return yes_response
-        print('Enter %s to set to `%s`, or anything else to accept the default value (`%s`): ' % (
-            _YES_CHOICES_STRING, yes_response, action.default))
-        response = input().strip()
+        response = get_input(prompt='Enter %s to set to `%s`, or anything else to accept the default value (`%s`):' % (
+            _YES_CHOICES_STRING, yes_response, action.default), strip=True)
         return yes_response if response in _YES_CHOICES else action.default
 
     elif action_type is _AppendConstAction:
         # this action type appends a constant value each time it is provided
         new_value = current_value if current_value else []
         while True:
-            print('Enter %s to append `%s` to the current value of `%s`, or anything else to skip: ' % (
-                _YES_CHOICES_STRING, action.const, new_value))
-            response = input().strip()
+            response = get_input(prompt='Enter %s to append `%s` to the current value of `%s`, or anything else to '
+                                        'skip:' % (_YES_CHOICES_STRING, action.const, new_value), strip=True)
             if response in _YES_CHOICES:
                 new_value.extend([action.const])
             else:
                 if action.required and action.const not in new_value:
                     print('This argument is required but has not been provided - adding `%s`' % action.const)
                     new_value.extend([action.const])
                 return new_value
@@ -163,45 +187,40 @@
             new_value = _parse_store_action(action, append=True)
         action.required = action_required
         return current_value if current_value else action.default
 
     elif action_type is _CountAction:
         # this action provides the number of times the same argument occurs
         while True:
-            print('Enter the number of times you would like to provide this argument, or leave blank to accept the '
-                  'default value (`%s`): ' % action.default)
-            count_response = input().strip()
+            count_response = get_input(prompt='Enter the number of times you would like to provide this argument, or '
+                                              'leave blank to accept the default value (`%s`):' % action.default,
+                                       strip=True)
             if count_response.isdigit():
                 return int(count_response)
             elif not count_response:
                 return action.default
 
     elif action_type is _StoreAction:
         # the default action type is able to handle one or more arguments flexibly
         return _parse_store_action(action)
 
-    else:
-        print('Tooey warning: action type', action_type, 'is not currently handled - skipping')
-
-    return action.default
-
 
 def _parse_store_action(action, append=False):
     new_value = []
     arg_num = 0
-    type_string = ' of type `%s`' % action.type.__name__ if action.type else ''
+    type_string = ' of type `%s`' % (
+        action.type.__name__ if hasattr(action.type, '__name__') else action.type) if action.type else ''
     choice_list_string = (' from `%s`' % ', '.join([str(c) for c in action.choices])) if action.choices else ''
     argument_required_string = 'This argument is required but has not been provided - please enter a value'
     while True:
         while True:
-            print('Enter %s%s%s for this argument, or leave blank to skip: ' % (
+            response = get_input(prompt='Enter %s%s%s for this argument, or leave blank to skip:' % (
                 'an additional value' if append else 'a value',
                 choice_list_string if choice_list_string else type_string if type_string else '',
-                (' to append to the current value `%s`' % new_value) if len(new_value) > 0 else ''))
-            response = input()
+                (' to append to the current value `%s`' % new_value) if len(new_value) > 0 else ''), strip=False)
             if response:
                 if action.type:
                     try:
                         response = action.type(response)
                     except ValueError:
                         print('The response entered (`%s`) is not of the required type - please enter a value of type '
                               '`%s`' % (response, action.type.__name__))
@@ -237,18 +256,22 @@
         if action.nargs == '?':
             # an optional single argument value, or its constant
             if not response:
                 if action.required:
                     print(argument_required_string)
                     continue
                 if action.const:
-                    print('This argument has a constant value (`%s`) - enter %s to choose this, or leave blank to '
-                          'accept the default (`%s`): ' % (action.const, _YES_CHOICES_STRING, action.default))
-                    if input().strip() in _YES_CHOICES:
+                    response = get_input(prompt='This argument has a constant value (`%s`) - enter %s to choose this, '
+                                                'leave blank to accept the default (`%s`), or enter anything else to '
+                                                'return to the previous prompt:' % (
+                                                    action.const, _YES_CHOICES_STRING, action.default), strip=True)
+                    if response in _YES_CHOICES:
                         return action.const
+                    elif response:
+                        continue
                 return action.default
             return response
 
         if action.nargs == '*':
             # a list of arguments (no minimum)
             if response:
                 continue
@@ -262,14 +285,8 @@
                 print(argument_required_string)
                 continue
             return new_value if new_value else action.default
 
 
 # ArgumentParser's exit_on_error argument was added in Python 3.9; we support below this so override rather than catch
 def error(self, message):
-    force_parser = argparse.ArgumentParser(add_help=False)
-    force_parser.add_argument('--force-tooey', action='store_true')
-    force_tooey = force_parser.parse_known_args()[0].force_tooey or os.environ.get('FORCE_TOOEY')
-    if sys.stdout.isatty() or force_tooey:
-        self.original_error_message = message  # to be used on failure/cancellation
-        return
-    self.original_error(message)
+    self.original_error_message = message  # to be used on failure/cancellation
```

### Comparing `tooey-0.2.0/tooey.egg-info/PKG-INFO` & `tooey-0.3.0/tooey.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tooey
-Version: 0.2.0
+Version: 0.3.0
 Summary: Automatically turn script arguments into an interactive terminal interface
 Home-page: https://github.com/simonrob/tooey
 Author: Simon Robinson
 Author-email: simon@robinson.ac
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/simonrob/tooey/issues
 Project-URL: Source Code, https://github.com/simonrob/tooey
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Terminals
@@ -88,9 +87,7 @@
 ```console
 $ FORCE_TOOEY=1 python tooey_example.py val1 --named-choices 1 3 | sort
 ```
 
 
 ## License
 [Apache 2.0](https://github.com/simonrob/tooey/blob/main/LICENSE)
-
-
```

