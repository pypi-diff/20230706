# Comparing `tmp/funcOAI-0.0.3.tar.gz` & `tmp/funcOAI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcOAI-0.0.3.tar", last modified: Sun Jul  2 00:25:30 2023, max compression
+gzip compressed data, was "funcOAI-0.0.4.tar", last modified: Thu Jul  6 19:46:46 2023, max compression
```

## Comparing `funcOAI-0.0.3.tar` & `funcOAI-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:25:30.599992 funcOAI-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 07:17:55.000000 funcOAI-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4798 2023-07-02 00:25:30.599992 funcOAI-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4107 2023-07-01 13:11:14.000000 funcOAI-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:25:30.599992 funcOAI-0.0.3/funcOAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4798 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:25:30.599992 funcOAI-0.0.3/functionalOAI/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-01 22:24:33.000000 funcOAI-0.0.3/functionalOAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-07-02 00:19:01.000000 funcOAI-0.0.3/functionalOAI/funAI.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-02 00:15:40.000000 funcOAI-0.0.3/functionalOAI/functions.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 00:25:30.599992 funcOAI-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-02 00:19:30.000000 funcOAI-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:46:46.305637 funcOAI-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 07:17:55.000000 funcOAI-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-07-06 19:46:46.305637 funcOAI-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6005 2023-07-05 15:15:02.000000 funcOAI-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:46:46.305637 funcOAI-0.0.4/funcOAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-07-06 19:46:46.000000 funcOAI-0.0.4/funcOAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-06 19:46:46.000000 funcOAI-0.0.4/funcOAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 19:46:46.000000 funcOAI-0.0.4/funcOAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-06 19:46:46.000000 funcOAI-0.0.4/funcOAI.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:46:46.305637 funcOAI-0.0.4/functionalOAI/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-06 16:48:01.000000 funcOAI-0.0.4/functionalOAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-07-06 19:45:00.000000 funcOAI-0.0.4/functionalOAI/funAI.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2023-07-06 16:53:06.000000 funcOAI-0.0.4/functionalOAI/functions.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 19:46:46.305637 funcOAI-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-06 19:46:32.000000 funcOAI-0.0.4/setup.py
```

### Comparing `funcOAI-0.0.3/LICENSE` & `funcOAI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funcOAI-0.0.3/PKG-INFO` & `funcOAI-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcOAI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that helps users easily create functions to feed to GPT function calling API
 Home-page: UNKNOWN
 Author: x5up0 aka.ryan
 Author-email: x5up0sbu@gmail.com
 License: UNKNOWN
 Keywords: python,OpenAI,ChatGPT,GPT API,function calling API,functions,openai-gpt
 Platform: UNKNOWN
@@ -122,14 +122,74 @@
 
 
 print(run_conversation())
 ```
 
 ### This is an edited example of the [official OpenAI API example](https://platform.openai.com/docs/guides/gpt/function-calling)
 
+
+## New Usage Feature
+
+-    You could now access all the elements inside the functions list and do all sort of list methods on them (most of them at least you could look in functions.py to see all the overridden list methods)
+```python
+from functionalOAI import FunAI
+
+client = FunAI()
+
+@client.attach
+def suM(a: int, b: int):
+    """return the sum of a and b"""
+    return a + b
+
+def muL(a: int, b: int):
+    """return the multiplication of a and b"""
+    return a * b
+
+print(client.functions)
+client.functions.append({"name": "muL", "description": "return the multiplication of a and b", ...})
+print(client.functions)
+```
+### Its made to make removing / adding / deleting functions easy
+
+```python
+# see if a function inside the list by the name or the body
+print("muL" in client.functions) # True
+
+# remove function by name (you could also add the whole body of the function)
+client.functions.remove("muL")
+
+print("muL" in client.functions) # False
+
+# remove a function using the del keyword
+del client.functions["muL"] # error since muL was already removed
+
+
+print(client.functions)
+
+# get the body of a specefic function by its name or its index in the list
+print(client.functions["suM"])
+
+# multiple ways to add a function
+client.functions.append({"name": "test", "description": "..."})
+client.functions.insert("at the index of a specefic function name or by the index", {"name": "test2", "description": "...."})
+print(client.functions)
+
+# replace a specefic function
+client.functions["test2"] = {"name": "test3", "description": "hackerman++"}
+
+# get the index of a specific function by its name or body
+client.functions.index("test3") # the index function calls another function called name_to_key so you could use that directly there is none special about index 
+
+# or get the name by the index
+client.functions.key_to_name(0) # suM
+
+# clear the whole list
+client.functions.clear()
+```
+
 ## NOTICE!!
 
 To make this module work correctly with all of you're functions there are set of rules you have to go by when defining the functions
 
 -    Providing type annotations for all the arguments e.g ...
 
 ```python
@@ -147,15 +207,15 @@
 ## WARNING
 
 -   This module is not fully complete as it still lacks some extra functionality
 -   There is no error handling as for now, so obeying the rules of function defining is necessary
 
 ## TODO
 
--    create a special type for the functions list, to make it more flexable and accessable, and much more efficient (handeling duplicates etc ...)
+-    ✅create a special type for the functions list, to make it more flexable and accessable, and much more efficient (handeling duplicates etc ...)
 -    create a multi-line docstring parser that gets a description for the function and a description for each of the arguments
 -    handle all possible errors in creating the body of the function, and create backup plans in case something was missing in the function definition
 
 ## Contribute
 
 ### You could contribute through
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `funcOAI-0.0.3/README.md` & `funcOAI-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -103,14 +103,74 @@
 
 
 print(run_conversation())
 ```
 
 ### This is an edited example of the [official OpenAI API example](https://platform.openai.com/docs/guides/gpt/function-calling)
 
+
+## New Usage Feature
+
+-    You could now access all the elements inside the functions list and do all sort of list methods on them (most of them at least you could look in functions.py to see all the overridden list methods)
+```python
+from functionalOAI import FunAI
+
+client = FunAI()
+
+@client.attach
+def suM(a: int, b: int):
+    """return the sum of a and b"""
+    return a + b
+
+def muL(a: int, b: int):
+    """return the multiplication of a and b"""
+    return a * b
+
+print(client.functions)
+client.functions.append({"name": "muL", "description": "return the multiplication of a and b", ...})
+print(client.functions)
+```
+### Its made to make removing / adding / deleting functions easy
+
+```python
+# see if a function inside the list by the name or the body
+print("muL" in client.functions) # True
+
+# remove function by name (you could also add the whole body of the function)
+client.functions.remove("muL")
+
+print("muL" in client.functions) # False
+
+# remove a function using the del keyword
+del client.functions["muL"] # error since muL was already removed
+
+
+print(client.functions)
+
+# get the body of a specefic function by its name or its index in the list
+print(client.functions["suM"])
+
+# multiple ways to add a function
+client.functions.append({"name": "test", "description": "..."})
+client.functions.insert("at the index of a specefic function name or by the index", {"name": "test2", "description": "...."})
+print(client.functions)
+
+# replace a specefic function
+client.functions["test2"] = {"name": "test3", "description": "hackerman++"}
+
+# get the index of a specific function by its name or body
+client.functions.index("test3") # the index function calls another function called name_to_key so you could use that directly there is none special about index 
+
+# or get the name by the index
+client.functions.key_to_name(0) # suM
+
+# clear the whole list
+client.functions.clear()
+```
+
 ## NOTICE!!
 
 To make this module work correctly with all of you're functions there are set of rules you have to go by when defining the functions
 
 -    Providing type annotations for all the arguments e.g ...
 
 ```python
@@ -128,15 +188,15 @@
 ## WARNING
 
 -   This module is not fully complete as it still lacks some extra functionality
 -   There is no error handling as for now, so obeying the rules of function defining is necessary
 
 ## TODO
 
--    create a special type for the functions list, to make it more flexable and accessable, and much more efficient (handeling duplicates etc ...)
+-    ✅create a special type for the functions list, to make it more flexable and accessable, and much more efficient (handeling duplicates etc ...)
 -    create a multi-line docstring parser that gets a description for the function and a description for each of the arguments
 -    handle all possible errors in creating the body of the function, and create backup plans in case something was missing in the function definition
 
 ## Contribute
 
 ### You could contribute through
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `funcOAI-0.0.3/funcOAI.egg-info/PKG-INFO` & `funcOAI-0.0.4/funcOAI.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcOAI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that helps users easily create functions to feed to GPT function calling API
 Home-page: UNKNOWN
 Author: x5up0 aka.ryan
 Author-email: x5up0sbu@gmail.com
 License: UNKNOWN
 Keywords: python,OpenAI,ChatGPT,GPT API,function calling API,functions,openai-gpt
 Platform: UNKNOWN
@@ -122,14 +122,74 @@
 
 
 print(run_conversation())
 ```
 
 ### This is an edited example of the [official OpenAI API example](https://platform.openai.com/docs/guides/gpt/function-calling)
 
+
+## New Usage Feature
+
+-    You could now access all the elements inside the functions list and do all sort of list methods on them (most of them at least you could look in functions.py to see all the overridden list methods)
+```python
+from functionalOAI import FunAI
+
+client = FunAI()
+
+@client.attach
+def suM(a: int, b: int):
+    """return the sum of a and b"""
+    return a + b
+
+def muL(a: int, b: int):
+    """return the multiplication of a and b"""
+    return a * b
+
+print(client.functions)
+client.functions.append({"name": "muL", "description": "return the multiplication of a and b", ...})
+print(client.functions)
+```
+### Its made to make removing / adding / deleting functions easy
+
+```python
+# see if a function inside the list by the name or the body
+print("muL" in client.functions) # True
+
+# remove function by name (you could also add the whole body of the function)
+client.functions.remove("muL")
+
+print("muL" in client.functions) # False
+
+# remove a function using the del keyword
+del client.functions["muL"] # error since muL was already removed
+
+
+print(client.functions)
+
+# get the body of a specefic function by its name or its index in the list
+print(client.functions["suM"])
+
+# multiple ways to add a function
+client.functions.append({"name": "test", "description": "..."})
+client.functions.insert("at the index of a specefic function name or by the index", {"name": "test2", "description": "...."})
+print(client.functions)
+
+# replace a specefic function
+client.functions["test2"] = {"name": "test3", "description": "hackerman++"}
+
+# get the index of a specific function by its name or body
+client.functions.index("test3") # the index function calls another function called name_to_key so you could use that directly there is none special about index 
+
+# or get the name by the index
+client.functions.key_to_name(0) # suM
+
+# clear the whole list
+client.functions.clear()
+```
+
 ## NOTICE!!
 
 To make this module work correctly with all of you're functions there are set of rules you have to go by when defining the functions
 
 -    Providing type annotations for all the arguments e.g ...
 
 ```python
@@ -147,15 +207,15 @@
 ## WARNING
 
 -   This module is not fully complete as it still lacks some extra functionality
 -   There is no error handling as for now, so obeying the rules of function defining is necessary
 
 ## TODO
 
--    create a special type for the functions list, to make it more flexable and accessable, and much more efficient (handeling duplicates etc ...)
+-    ✅create a special type for the functions list, to make it more flexable and accessable, and much more efficient (handeling duplicates etc ...)
 -    create a multi-line docstring parser that gets a description for the function and a description for each of the arguments
 -    handle all possible errors in creating the body of the function, and create backup plans in case something was missing in the function definition
 
 ## Contribute
 
 ### You could contribute through
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `funcOAI-0.0.3/functionalOAI/functions.py` & `funcOAI-0.0.4/functionalOAI/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 class functionsList(list):
     def __init__(self):
         self.__types = (dict, Dict)
         self.__map   = dict() 
 
     def __getitem__(self, val: Union[str, int]) -> Dict:
         if isinstance(val, str):
-            ntk = self.name_to_key(val)
-            return super().__getitem__(ntk)
+            return self.__map[val]
 
         return super().__getitem__(val)
 
     def __contains__(self, val: Union[dict, str]) -> bool:
         if isinstance(val, str):
             try:
                 ntk = self.name_to_key(val)
```

### Comparing `funcOAI-0.0.3/setup.py` & `funcOAI-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A package that helps users easily create functions to feed to GPT function calling API'
 # Setting up
 setup(
     name="funcOAI",
     version=VERSION,
     author="x5up0 aka.ryan",
     author_email="x5up0sbu@gmail.com",
```

