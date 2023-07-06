# Comparing `tmp/domini-0.8.1.tar.gz` & `tmp/domini-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domini-0.8.1.tar", max compression
+gzip compressed data, was "domini-0.9.0.tar", max compression
```

## Comparing `domini-0.8.1.tar` & `domini-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.8.1/LICENSE
--rw-r--r--   0        0        0     2070 2023-06-08 23:04:06.895144 domini-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.8.1/domini/__init__.py
--rw-r--r--   0        0        0       19 2023-06-08 14:31:26.952321 domini-0.8.1/domini/html/__init__.py
--rw-r--r--   0        0        0     2139 2023-06-08 22:40:23.979848 domini-0.8.1/domini/html/events.py
--rw-r--r--   0        0        0    16294 2023-06-20 15:40:16.828970 domini-0.8.1/domini/html/tags.py
--rw-r--r--   0        0        0      418 2023-06-20 15:41:24.028094 domini-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 domini-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2070 2023-06-08 23:04:06.895144 domini-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.9.0/domini/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-08 14:31:26.952321 domini-0.9.0/domini/html/__init__.py
+-rw-r--r--   0        0        0     2139 2023-06-08 22:40:23.979848 domini-0.9.0/domini/html/events.py
+-rw-r--r--   0        0        0    16864 2023-06-20 16:37:37.192036 domini-0.9.0/domini/html/tags.py
+-rw-r--r--   0        0        0      418 2023-06-20 16:38:53.244314 domini-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 domini-0.9.0/PKG-INFO
```

### Comparing `domini-0.8.1/LICENSE` & `domini-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domini-0.8.1/README.md` & `domini-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `domini-0.8.1/domini/html/events.py` & `domini-0.9.0/domini/html/events.py`

 * *Files identical despite different names*

### Comparing `domini-0.8.1/domini/html/tags.py` & `domini-0.9.0/domini/html/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,29 @@
         # and have its elements added
         if isinstance(content, Iterable):
             return copy.add(*content)
         
         # o) Anything else, add it singularly
         return copy.add(content)
 
+    def __pow__(self, content: Content, /) -> HTMLTag:
+        """
+        Return a copy with the children added.
+        This is a right-handed alternative to using greater-than.
+
+        It can be used in situations such as;
+            body()> (main()> (p()> 'Hello, World!'))
+        to mitigate parentheses that make it harder to read.
+            body()** main()** p()** 'Hello, World!'
+
+        This isn't as pretty and HTML-like as using greater-than,
+        but the option is there if you want to reduce parentheses.
+        """
+        return self > content
+
     def __contains__(self, attribute: str, /) -> bool:
         """
         Get whether tag has attribute.
         """
         return attribute in self.attrs \
             or attribute in self.kwattrs
```

### Comparing `domini-0.8.1/PKG-INFO` & `domini-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domini
-Version: 0.8.1
+Version: 0.9.0
 Summary: Create HTML documents using Pythonic syntax that mimics the real deal.
 Home-page: https://gitlab.com/deepadmax/domini
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

