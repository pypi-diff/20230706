# Comparing `tmp/foma_bindings-0.1.3.tar.gz` & `tmp/foma_bindings-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foma_bindings-0.1.3.tar", last modified: Fri Jun 30 02:28:27 2023, max compression
+gzip compressed data, was "foma_bindings-0.1.4.tar", last modified: Thu Jul  6 16:28:16 2023, max compression
```

## Comparing `foma_bindings-0.1.3.tar` & `foma_bindings-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.3/LICENSE.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3786 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     2986 2023-06-23 15:26:24.000000 foma_bindings-0.1.3/README.md
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/foma_bindings/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     4769 2023-06-23 12:54:26.000000 foma_bindings-0.1.3/foma_bindings/__init__.py
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/foma_bindings/fst/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    15492 2023-06-30 02:04:05.000000 foma_bindings-0.1.3/foma_bindings/fst/__init__.py
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/foma_bindings/mtfst/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     6343 2023-06-22 18:17:49.000000 foma_bindings-0.1.3/foma_bindings/mtfst/__init__.py
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/foma_bindings.egg-info/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3786 2023-06-30 02:28:27.000000 foma_bindings-0.1.3/foma_bindings.egg-info/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      281 2023-06-30 02:28:27.000000 foma_bindings-0.1.3/foma_bindings.egg-info/SOURCES.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-30 02:28:27.000000 foma_bindings-0.1.3/foma_bindings.egg-info/dependency_links.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       14 2023-06-30 02:28:27.000000 foma_bindings-0.1.3/foma_bindings.egg-info/top_level.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.3/pyproject.toml
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-06-30 02:28:27.733139 foma_bindings-0.1.3/setup.cfg
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1663 2023-06-30 02:24:38.000000 foma_bindings-0.1.3/setup.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.4/LICENSE.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3849 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3049 2023-07-06 16:28:10.000000 foma_bindings-0.1.4/README.md
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/foma_bindings/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     4769 2023-06-23 12:54:26.000000 foma_bindings-0.1.4/foma_bindings/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/foma_bindings/fst/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    17667 2023-07-06 16:18:20.000000 foma_bindings-0.1.4/foma_bindings/fst/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/foma_bindings/mtfst/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     6343 2023-06-22 18:17:49.000000 foma_bindings-0.1.4/foma_bindings/mtfst/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/foma_bindings.egg-info/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3849 2023-07-06 16:28:16.000000 foma_bindings-0.1.4/foma_bindings.egg-info/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      281 2023-07-06 16:28:16.000000 foma_bindings-0.1.4/foma_bindings.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-07-06 16:28:16.000000 foma_bindings-0.1.4/foma_bindings.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       14 2023-07-06 16:28:16.000000 foma_bindings-0.1.4/foma_bindings.egg-info/top_level.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.4/pyproject.toml
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-07-06 16:28:16.597948 foma_bindings-0.1.4/setup.cfg
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1663 2023-07-06 16:27:52.000000 foma_bindings-0.1.4/setup.py
```

### Comparing `foma_bindings-0.1.3/LICENSE.txt` & `foma_bindings-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.3/PKG-INFO` & `foma_bindings-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foma_bindings
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
@@ -52,9 +52,11 @@
 
 - extensive readability edits have been made, including splitting classes into separate files, alphabetizing the C API mappings, and extensive renaming of function and variable names
 - `get_alphabet` and the aliased `get_sigma` functions have been added
 - the multi-tape FST class/section has been entirely commented out for now
 - additional printing parameters have been added, such as printing with flags included
 - the files have been made ready for distribution on `pip`
 - apache copyright notices have been added to all the relevant python files
+- add query function
+- add function to get the flag diacritics
```

### Comparing `foma_bindings-0.1.3/README.md` & `foma_bindings-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,7 +31,9 @@
 
 - extensive readability edits have been made, including splitting classes into separate files, alphabetizing the C API mappings, and extensive renaming of function and variable names
 - `get_alphabet` and the aliased `get_sigma` functions have been added
 - the multi-tape FST class/section has been entirely commented out for now
 - additional printing parameters have been added, such as printing with flags included
 - the files have been made ready for distribution on `pip`
 - apache copyright notices have been added to all the relevant python files
+- add query function
+- add function to get the flag diacritics
```

### Comparing `foma_bindings-0.1.3/foma_bindings/__init__.py` & `foma_bindings-0.1.4/foma_bindings/__init__.py`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.3/foma_bindings/fst/__init__.py` & `foma_bindings-0.1.4/foma_bindings/fst/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from foma_bindings import *
 from sys import maxsize
 from ctypes import c_bool
+import re
+
+# This regex matches all foma flag diacritics.
+# https://giellalt.uit.no/lang/sme/docu-sme-flag-diacritics.html
+# Flag diacritic example: @P.Name.Value@
+# Valid flag operators: P, R, D, U, C, N.
+# Value part is optional.
+MATCH_NAME = 'full_flag'
+FLAGS_REGEX = re.compile(f'(?P<{MATCH_NAME}>@[PRDUCN][.][^@.\s]+([.][^@.\s]+)?@)')
 
 class Fst:
     '''
     This class loads a compiled foma binary into memory, and allows operations on it.
 
     Here is an example of use:
 
@@ -43,14 +52,15 @@
         - apply_up
         - lower_words
         - upper_words
         - words
 
     FST Functions:
         - get_alphabet
+        - get_flag_diacritics
         - union
         - intersect
         - minus
         - concatenate
         - compose
         - lower
         - upper
@@ -62,16 +72,18 @@
 
     # This is the symbol to split a word on tokens, i.e. "fox+V" becomes ['f','o','x','+V'].
     _TOKENIZE_SYMBOL = b'\x07'
 
     # Bit flags for different options when printing output.
     # TODO PRINT_SPACES and TOKENIZE do not mesh well together. What to do?
     NO_FLAGS = 0
-    PRINT_SPACES = 1
-    PRINT_FLAGS = 2
+    SHOW_SPACES = 1
+    PRINT_SPACES = SHOW_SPACES
+    SHOW_FLAGS = 2
+    PRINT_FLAGS = SHOW_FLAGS
     TOKENIZE = 4
     VERBOSE = TOKENIZE | PRINT_FLAGS
 
     #region Class and Static Methods
     @classmethod
     def define(cls, definition, name):
         '''Defines an FSM constant; can be supplied regex or existing FSM.
@@ -253,14 +265,20 @@
         sigma = Fst()
         sigma.fst_handle = self._foma_call_unary(foma_fsm_sigma_net, minimize)
         return sigma.words(flags)
     
     # Alias to get_alphabet since both are very different yet valid names for the same function.
     get_sigma = get_alphabet
 
+    def get_flag_diacritics(self, minimize=True):
+        '''Returns a list of all the flag diacritics in the FST.'''
+        alphabet = ' '.join(self.get_alphabet(minimize, flags=Fst.SHOW_FLAGS))
+        flag_diacritics = [match.groupdict()[MATCH_NAME] for match in FLAGS_REGEX.finditer(alphabet)]
+        return flag_diacritics
+
     def union(self, other, minimize=True):
         '''Returns the union of two FSTs.'''
         fst = Fst()
         fst.fst_handle = self._foma_call_binary(other, foma_fsm_union, minimize)
         return fst
 
     def intersect(self, other, minimize=True):
@@ -305,15 +323,15 @@
     
     #endregion
 
     #region Dunders
     def __init__(self, regex=False):
         if regex:
             self.regex = self.encode(regex)
-            self.fst_handle = foma_fsm_parse_regex(c_char_p(self.regex), c_void_p(self._network_definitions.defined_handle), c_void_p(self._function_definitions.deffhandle))
+            self.fst_handle = foma_fsm_parse_regex(c_char_p(self.regex), c_void_p(self._network_definitions.defined_handle), c_void_p(self._function_definitions.defined_handle))
             if not self.fst_handle:
                 raise ValueError("Syntax error in regex")
         else:
             self.fst_handle = None
         self.get_item_applyer = None
 
     def __getitem__(self, key):
@@ -417,7 +435,43 @@
         fst.fst_handle = self._foma_call_unary(foma_fsm_complement)
         return fst
 
     def __iter__(self):
         return self._apply(foma_apply_upper_words, word=None, flags=Fst.NO_FLAGS)
     
     #endregion
+    
+    #region String Matching
+
+    def query(self, stem:str, flag_diacritics:list[str] | None = None, **kwargs) -> list[str] | None:
+        '''kwargs should be the feature names and feature values, i.e. {polarity: [POS, NEG]}, or {SUBJECT: None}. This list must be appropriately ordered and exhaustive.'''
+        # TODO make the docstring better.
+
+        # We'll use this expression to freely insert flag diacritics into the query.
+        if flag_diacritics is not None:
+            flag_diacritics = " | ".join([f'"{flag}"' for flag in flag_diacritics])
+
+        # Build query.
+        query_builder = '{%s}' % stem
+
+        # Loop over tags and create the query.
+        for tags in kwargs.values():
+            print(tags)
+            if tags is None:
+                query_builder += '[ ? ]'
+            else:
+                tagging_options = [f'"+{tag}"' for tag in tags]
+                query_builder += f"[ {' | '.join(tagging_options)} ]"
+
+        query = f'[ {query_builder} ]'
+
+        # Freely insert flag diacritics into the query. Needed for composition.
+        if flag_diacritics is not None:
+            query += f' / [ {flag_diacritics} ]'
+
+        selector_fst = Fst(query)
+
+        # Apply query to fst and return generator of the analyses.
+        resulting_fst = selector_fst.compose(self)
+        return zip(resulting_fst.upper_words(), resulting_fst.lower_words())
+
+    #endregion
```

### Comparing `foma_bindings-0.1.3/foma_bindings/mtfst/__init__.py` & `foma_bindings-0.1.4/foma_bindings/mtfst/__init__.py`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.3/foma_bindings.egg-info/PKG-INFO` & `foma_bindings-0.1.4/foma_bindings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foma-bindings
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
@@ -52,9 +52,11 @@
 
 - extensive readability edits have been made, including splitting classes into separate files, alphabetizing the C API mappings, and extensive renaming of function and variable names
 - `get_alphabet` and the aliased `get_sigma` functions have been added
 - the multi-tape FST class/section has been entirely commented out for now
 - additional printing parameters have been added, such as printing with flags included
 - the files have been made ready for distribution on `pip`
 - apache copyright notices have been added to all the relevant python files
+- add query function
+- add function to get the flag diacritics
```

### Comparing `foma_bindings-0.1.3/setup.py` & `foma_bindings-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name='foma_bindings',
-    version='0.1.3',
+    version='0.1.4',
     description='Python bindings for the foma finite-state technology suite',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/CultureFoundryCA/foma_bindings',
     author='CultureFoundry',
     author_email='info@culturefoundrystudios.com',
     license='Apache 2.0',
```

