# Comparing `tmp/python-barcode-0.8.3.tar.gz` & `tmp/python-barcode-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-barcode-0.8.3.tar", last modified: Fri May 11 17:53:16 2018, max compression
+gzip compressed data, was "dist/python-barcode-0.9.0.tar", last modified: Thu Jun 14 16:50:08 2018, max compression
```

## Comparing `python-barcode-0.8.3.tar` & `python-barcode-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/barcode/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/barcode/charsets/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/charsets/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2896 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/charsets/code128.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1264 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/charsets/code39.py
--rw-r--r--   0 travis    (2000) travis    (2000)      634 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/charsets/ean.py
--rw-r--r--   0 travis    (2000) travis    (2000)      262 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/charsets/itf.py
--rw-r--r--   0 travis    (2000) travis    (2000)      370 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/charsets/upc.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)   321524 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/DejaVuSansMono.ttf
--rwxr-xr-x   0 travis    (2000) travis    (2000)     1946 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/__init__.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     3266 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/base.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     7743 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/codex.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     5676 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/ean.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)      714 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/errors.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     3838 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/isxn.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2280 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/itf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4142 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/pybarcode.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     2918 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/upc.py
--rw-r--r--   0 travis    (2000) travis    (2000)      116 2018-05-11 17:53:16.000000 python-barcode-0.8.3/barcode/version.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)    11991 2018-05-11 17:52:23.000000 python-barcode-0.8.3/barcode/writer.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/docs/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/docs/images/
--rwxr-xr-x   0 travis    (2000) travis    (2000)     3802 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/images/pybarcode.png
--rw-r--r--   0 travis    (2000) travis    (2000)     1517 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/images/pybarcode_small.png
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/docs/writers/
--rwxr-xr-x   0 travis    (2000) travis    (2000)      461 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/writers/create_writer.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)      588 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/writers/image.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)     1686 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/writers/index.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)      339 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/writers/svg.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)     3222 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/Makefile
--rwxr-xr-x   0 travis    (2000) travis    (2000)     1736 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/barcode.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     1869 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/codes.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      830 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/commandline.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)     6671 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/conf.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)      611 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     1252 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/license.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)     3190 2018-05-11 17:52:23.000000 python-barcode-0.8.3/docs/make.bat
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     7653 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      965 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       59 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       17 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        8 2018-05-11 17:53:16.000000 python-barcode-0.8.3/python_barcode.egg-info/top_level.txt
--rwxr-xr-x   0 travis    (2000) travis    (2000)      148 2018-05-11 17:52:23.000000 python-barcode-0.8.3/.gitignore
--rw-r--r--   0 travis    (2000) travis    (2000)      617 2018-05-11 17:52:23.000000 python-barcode-0.8.3/.travis.yml
--rwxr-xr-x   0 travis    (2000) travis    (2000)      206 2018-05-11 17:52:23.000000 python-barcode-0.8.3/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     5066 2018-05-11 17:52:23.000000 python-barcode-0.8.3/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     4095 2018-05-11 17:52:23.000000 python-barcode-0.8.3/example-ean13.png
--rwxr-xr-x   0 travis    (2000) travis    (2000)     1428 2018-05-11 17:52:23.000000 python-barcode-0.8.3/setup.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     4798 2018-05-11 17:52:23.000000 python-barcode-0.8.3/test.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7653 2018-05-11 17:53:16.000000 python-barcode-0.8.3/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-05-11 17:53:16.000000 python-barcode-0.8.3/setup.cfg
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/barcode/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/barcode/charsets/
+-rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/charsets/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2896 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/charsets/code128.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1264 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/charsets/code39.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      634 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/charsets/ean.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      262 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/charsets/itf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      370 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/charsets/upc.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)   321524 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/DejaVuSansMono.ttf
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     1946 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/__init__.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     3236 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/base.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     7753 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/codex.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     5676 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/ean.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      714 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/errors.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     3838 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/isxn.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2280 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/itf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     4188 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/pybarcode.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     2918 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/upc.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      116 2018-06-14 16:50:08.000000 python-barcode-0.9.0/barcode/version.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)    11991 2018-06-14 16:49:51.000000 python-barcode-0.9.0/barcode/writer.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/docs/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/docs/images/
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     3802 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/images/pybarcode.png
+-rw-r--r--   0 travis    (2000) travis    (2000)     1517 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/images/pybarcode_small.png
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/docs/writers/
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      461 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/writers/create_writer.rst
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      588 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/writers/image.rst
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     1686 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/writers/index.rst
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      339 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/writers/svg.rst
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     3222 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/Makefile
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     1736 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/barcode.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     1869 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/codes.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)      830 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/commandline.rst
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     6671 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/conf.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      611 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/index.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     1252 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/license.rst
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     3190 2018-06-14 16:49:51.000000 python-barcode-0.9.0/docs/make.bat
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     7653 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      973 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       59 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       17 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        8 2018-06-14 16:50:08.000000 python-barcode-0.9.0/python_barcode.egg-info/top_level.txt
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      148 2018-06-14 16:49:51.000000 python-barcode-0.9.0/.gitignore
+-rw-r--r--   0 travis    (2000) travis    (2000)      617 2018-06-14 16:49:51.000000 python-barcode-0.9.0/.travis.yml
+-rw-r--r--   0 travis    (2000) travis    (2000)     1135 2018-06-14 16:49:51.000000 python-barcode-0.9.0/LICENCE
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      206 2018-06-14 16:49:51.000000 python-barcode-0.9.0/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     5066 2018-06-14 16:49:51.000000 python-barcode-0.9.0/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)     4095 2018-06-14 16:49:51.000000 python-barcode-0.9.0/example-ean13.png
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     1428 2018-06-14 16:49:51.000000 python-barcode-0.9.0/setup.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     4798 2018-06-14 16:49:51.000000 python-barcode-0.9.0/test.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7653 2018-06-14 16:50:08.000000 python-barcode-0.9.0/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-06-14 16:50:08.000000 python-barcode-0.9.0/setup.cfg
```

### Comparing `python-barcode-0.8.3/barcode/charsets/code128.py` & `python-barcode-0.9.0/barcode/charsets/code128.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/charsets/code39.py` & `python-barcode-0.9.0/barcode/charsets/code39.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/charsets/ean.py` & `python-barcode-0.9.0/barcode/charsets/ean.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/DejaVuSansMono.ttf` & `python-barcode-0.9.0/barcode/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/__init__.py` & `python-barcode-0.9.0/barcode/__init__.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/base.py` & `python-barcode-0.9.0/barcode/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from barcode.writer import SVGWriter
 
 
 class Barcode(object):
 
     name = ''
 
-    raw = None
-
     digits = 0
 
     default_writer = SVGWriter
 
     default_writer_options = {
         'module_width': 0.2,
         'module_height': 15.0,
@@ -109,9 +107,9 @@
         if options['write_text'] or text is not None:
             if text is not None:
                 options['text'] = text
             else:
                 options['text'] = self.get_fullcode()
         self.writer.set_options(options)
         code = self.build()
-        raw = Barcode.raw = self.writer.render(code)
+        raw = self.writer.render(code)
         return raw
```

### Comparing `python-barcode-0.8.3/barcode/codex.py` & `python-barcode-0.9.0/barcode/codex.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def build(self):
         chars = [code39.EDGE]
         for char in self.code:
             chars.append(code39.MAP[char][1])
         chars.append(code39.EDGE)
         return [code39.MIDDLE.join(chars)]
 
-    def render(self, writer_options, text=None):
+    def render(self, writer_options=None, text=None):
         options = dict(module_width=MIN_SIZE, quiet_zone=MIN_QUIET_ZONE)
         options.update(writer_options or {})
         return Barcode.render(self, options, text)
 
 
 class PZN7(Code39):
     """Initializes new German number for pharmaceutical products.
@@ -248,15 +248,15 @@
         code = ''
         for code_num in encoded:
             code += code128.CODES[code_num]
         code += code128.STOP
         code += '11'
         return [code]
 
-    def render(self, writer_options, text=None):
+    def render(self, writer_options=None, text=None):
         options = dict(module_width=MIN_SIZE, quiet_zone=MIN_QUIET_ZONE)
         options.update(writer_options or {})
         return Barcode.render(self, options, text)
 
 
 # For pre 0.8 compatibility
 PZN = PZN7
```

### Comparing `python-barcode-0.8.3/barcode/ean.py` & `python-barcode-0.9.0/barcode/ean.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/errors.py` & `python-barcode-0.9.0/barcode/errors.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/isxn.py` & `python-barcode-0.9.0/barcode/isxn.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/itf.py` & `python-barcode-0.9.0/barcode/itf.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/pybarcode.py` & `python-barcode-0.9.0/barcode/pybarcode.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,16 @@
         gui_parser = subparsers.add_parser('gui', help='Opens a simple '
                                            'PyQt GUI to create barcodes.')
         gui_parser.set_defaults(func=open_gui)
     create_parser.set_defaults(type='svg', compress=False, func=create_barcode,
                                barcode='code39', text=None)
     args = parser.parse_args()
     try:
-        args.func(args, parser)
+        func = args.func
     except AttributeError:
-        print("Use --help to see help")
+        parser.error("You need to tell me what to do.")
+    else:
+        func(args, parser)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `python-barcode-0.8.3/barcode/upc.py` & `python-barcode-0.9.0/barcode/upc.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/barcode/writer.py` & `python-barcode-0.9.0/barcode/writer.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/images/pybarcode.png` & `python-barcode-0.9.0/docs/images/pybarcode.png`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/images/pybarcode_small.png` & `python-barcode-0.9.0/docs/images/pybarcode_small.png`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/writers/image.rst` & `python-barcode-0.9.0/docs/writers/image.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/writers/index.rst` & `python-barcode-0.9.0/docs/writers/index.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/Makefile` & `python-barcode-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/barcode.rst` & `python-barcode-0.9.0/docs/barcode.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/codes.rst` & `python-barcode-0.9.0/docs/codes.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/commandline.rst` & `python-barcode-0.9.0/docs/commandline.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/conf.py` & `python-barcode-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/index.rst` & `python-barcode-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/license.rst` & `python-barcode-0.9.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/docs/make.bat` & `python-barcode-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/python_barcode.egg-info/PKG-INFO` & `python-barcode-0.9.0/python_barcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-barcode
-Version: 0.8.3
+Version: 0.9.0
 Summary: Create standard barcodes with Python. No external modules needed (optional PIL support included).
 Home-page: https://github.com/WhyNotHugo/python-barcode
 Author: Thorsten Weimann et al
 Author-email: weimann.th@yahoo.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: python-barcode
```

### Comparing `python-barcode-0.8.3/python_barcode.egg-info/SOURCES.txt` & `python-barcode-0.9.0/python_barcode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .travis.yml
+LICENCE
 MANIFEST.in
 README.rst
 example-ean13.png
 setup.py
 test.py
 barcode/DejaVuSansMono.ttf
 barcode/__init__.py
```

### Comparing `python-barcode-0.8.3/.travis.yml` & `python-barcode-0.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/README.rst` & `python-barcode-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/example-ean13.png` & `python-barcode-0.9.0/example-ean13.png`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/setup.py` & `python-barcode-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/test.py` & `python-barcode-0.9.0/test.py`

 * *Files identical despite different names*

### Comparing `python-barcode-0.8.3/PKG-INFO` & `python-barcode-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-barcode
-Version: 0.8.3
+Version: 0.9.0
 Summary: Create standard barcodes with Python. No external modules needed (optional PIL support included).
 Home-page: https://github.com/WhyNotHugo/python-barcode
 Author: Thorsten Weimann et al
 Author-email: weimann.th@yahoo.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: python-barcode
```

