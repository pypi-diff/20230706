# Comparing `tmp/anyon-3.5.4-cp311-none-win_amd64.whl.zip` & `tmp/anyon-3.5.5-cp311-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 363082 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jul-02 00:40 anyon-3.5.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2318 b- defN 23-Jul-02 00:40 anyon-3.5.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-02 00:40 anyon-3.5.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-02 00:40 anyon-3.5.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 23-Jul-02 00:40 anyon-3.5.4.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-Jul-02 00:39 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    81920 b- defN 23-Jul-02 00:39 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   101376 b- defN 23-Jul-02 00:39 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   154112 b- defN 23-Jul-02 00:39 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Jul-02 00:39 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    94208 b- defN 23-Jul-02 00:39 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   144384 b- defN 23-Jul-02 00:39 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    62976 b- defN 23-Jul-02 00:39 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   115200 b- defN 23-Jul-02 00:39 anyon/stage/device.pyd
-14 files, 799523 bytes uncompressed, 361320 bytes compressed:  54.8%
+Zip file size: 864223 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-05 23:55 anyon-3.5.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-05 23:55 anyon-3.5.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 23-Jul-05 23:55 anyon-3.5.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-05 23:55 anyon-3.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      376 b- defN 23-Jul-05 23:55 anyon-3.5.5.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122299 b- defN 23-Jul-05 23:54 anyon/__init__.so
+-rwxr-xr-x  2.0 unx   326281 b- defN 23-Jul-05 23:54 anyon/loader.so
+-rwxr-xr-x  2.0 unx   364057 b- defN 23-Jul-05 23:54 anyon/remote.so
+-rwxr-xr-x  2.0 unx   539897 b- defN 23-Jul-05 23:54 anyon/server.so
+-rwxr-xr-x  2.0 unx   122683 b- defN 23-Jul-05 23:55 anyon/stage/__init__.so
+-rwxr-xr-x  2.0 unx   328381 b- defN 23-Jul-05 23:55 anyon/stage/calculator.so
+-rwxr-xr-x  2.0 unx   511883 b- defN 23-Jul-05 23:55 anyon/stage/compiler.so
+-rwxr-xr-x  2.0 unx   240142 b- defN 23-Jul-05 23:55 anyon/stage/demodulator.so
+-rwxr-xr-x  2.0 unx   396441 b- defN 23-Jul-05 23:55 anyon/stage/device.so
+14 files, 2955881 bytes uncompressed, 862479 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-3.5.4.dist-info/LICENSE
+Filename: anyon-3.5.5.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.5.4.dist-info/METADATA
+Filename: anyon-3.5.5.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.5.4.dist-info/WHEEL
+Filename: anyon-3.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.5.4.dist-info/top_level.txt
+Filename: anyon-3.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.5.4.dist-info/RECORD
+Filename: anyon-3.5.5.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.pyd
+Filename: anyon/__init__.so
 Comment: 
 
-Filename: anyon/loader.pyd
+Filename: anyon/loader.so
 Comment: 
 
-Filename: anyon/remote.pyd
+Filename: anyon/remote.so
 Comment: 
 
-Filename: anyon/server.pyd
+Filename: anyon/server.so
 Comment: 
 
-Filename: anyon/stage/__init__.pyd
+Filename: anyon/stage/__init__.so
 Comment: 
 
-Filename: anyon/stage/calculator.pyd
+Filename: anyon/stage/calculator.so
 Comment: 
 
-Filename: anyon/stage/compiler.pyd
+Filename: anyon/stage/compiler.so
 Comment: 
 
-Filename: anyon/stage/demodulator.pyd
+Filename: anyon/stage/demodulator.so
 Comment: 
 
-Filename: anyon/stage/device.pyd
+Filename: anyon/stage/device.so
 Comment: 
 
 Zip file comment:
```

## Comparing `anyon-3.5.4.dist-info/METADATA` & `anyon-3.5.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-Metadata-Version: 2.1
-Name: anyon
-Version: 3.5.4
-Summary: Dream It Possible!
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: axion (>=3.4.5)
-Requires-Dist: srpc (>=4.2.8)
-Requires-Dist: zee (>=0.0.3)
-Requires-Dist: requests (>=2.28.0)
-
+Metadata-Version: 2.1
+Name: anyon
+Version: 3.5.5
+Summary: Dream It Possible!
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: axion (>=3.4.5)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.3)
+Requires-Dist: requests (>=2.28.0)
+
```

