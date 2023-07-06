# Comparing `tmp/gptfunctionutil-0.1.4.tar.gz` & `tmp/gptfunctionutil-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfunctionutil-0.1.4.tar", last modified: Wed Jul  5 20:01:57 2023, max compression
+gzip compressed data, was "gptfunctionutil-0.1.6.tar", last modified: Thu Jul  6 19:21:19 2023, max compression
```

## Comparing `gptfunctionutil-0.1.4.tar` & `gptfunctionutil-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.340661 gptfunctionutil-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/.github/workflows/publishpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/pytest.local.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/src/gptfunctionutil/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/src/gptfunctionutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/src/gptfunctionutil/functionlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/src/gptfunctionutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-05 20:01:57.000000 gptfunctionutil-0.1.4/src/gptfunctionutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 20:01:57.000000 gptfunctionutil-0.1.4/src/gptfunctionutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:01:57.000000 gptfunctionutil-0.1.4/src/gptfunctionutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-05 20:01:57.000000 gptfunctionutil-0.1.4/src/gptfunctionutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 20:01:57.000000 gptfunctionutil-0.1.4/src/gptfunctionutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:57.344661 gptfunctionutil-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-05 20:01:33.000000 gptfunctionutil-0.1.4/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.507264 gptfunctionutil-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.499263 gptfunctionutil-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.github/workflows/publishpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/pytest.local.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:21:19.507264 gptfunctionutil-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/src/gptfunctionutil/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/src/gptfunctionutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/src/gptfunctionutil/functionlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/tests/test_methods.py
```

### Comparing `gptfunctionutil-0.1.4/.github/workflows/publishpackage.yaml` & `gptfunctionutil-0.1.6/.github/workflows/publishpackage.yaml`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.4/.gitignore` & `gptfunctionutil-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.4/.vscode/settings.json` & `gptfunctionutil-0.1.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.4/LICENSE` & `gptfunctionutil-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.4/pyproject.toml` & `gptfunctionutil-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = 'gptfunctionutil'
-version = "0.1.4"
+version = "0.1.6"
 license = {file = "LICENSE"}
 authors = [{name="Crosswave Omega",email= "xtream2pro@gmail.com"}]
 description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API"
 readme = 'README.md'
 
 keywords = ['discord.py', 'OpenAI', 'Function Calling API']
 requires-python = '>=3.10'
 
 dependencies = [
-    "discord>=2.3.1"
+    "discord>=2.1.0"
 ]
 [project.urls]
 "Homepage"= "https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility"
 
 
 [options.packages.find]
 exclude = ['tests',  'docs']
```

### Comparing `gptfunctionutil-0.1.4/src/gptfunctionutil/functionlib.py` & `gptfunctionutil-0.1.6/src/gptfunctionutil/functionlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Command,
     Context,
     Bot,
     CommandNotFound,
     CheckFailure
 )
 
-def hello_world():
-    print("tester")
 
 class CommandSingleton:
     _instance = None
     _commands = {}
 
     @classmethod
     def get_instance(cls):
@@ -125,14 +123,15 @@
                 comm=method.libcommand
                 if comm.enabled:
                     schema=comm.function_schema
             if schema!=None:
                 if schema.get('parameters',None)!=None:
                     functions_with_schema.append(schema)
         return functions_with_schema
+
     def expression_match(self, function_args: str):
         '''because sometimes, the API returns an expression and not a single integer.'''
         if self.do_expression and self.my_math_parser!=None:
             '''In case I want to change how I want to parse expressions later.'''
             expression_detect_pattern = r'(?<=:\s)([^"]*?[+\-*/][^"]*?)(?=(?:,|\s*\}))'
             return re.sub(expression_detect_pattern, lambda m: self.my_math_parser(m.group()), function_args)
         return function_args
```

### Comparing `gptfunctionutil-0.1.4/tests/conftest.py` & `gptfunctionutil-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.4/tests/test_methods.py` & `gptfunctionutil-0.1.6/tests/test_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,13 +64,15 @@
         registered_commands = []
         for command in bot.walk_commands():
             registered_commands.append(command.name)
         assert 'test_command' in registered_commands
         assert 'test_command' in schema
         assert 'noninvoke_test_command' in registered_commands
 
+
+
 # Example usage of the bot fixture
 @pytest.mark.asyncio
 async def test_bot(bot):
     async for bot in bot:
         assert bot is not None
         assert isinstance(bot, commands.Bot)
```

