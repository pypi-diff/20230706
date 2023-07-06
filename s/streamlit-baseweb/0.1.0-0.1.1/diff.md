# Comparing `tmp/streamlit_baseweb-0.1.0.tar.gz` & `tmp/streamlit_baseweb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_baseweb-0.1.0.tar", last modified: Thu Jul  6 00:11:51 2023, max compression
+gzip compressed data, was "streamlit_baseweb-0.1.1.tar", last modified: Thu Jul  6 00:17:08 2023, max compression
```

## Comparing `streamlit_baseweb-0.1.0.tar` & `streamlit_baseweb-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.144582 streamlit_baseweb-0.1.0/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      101 2023-07-06 00:06:11.000000 streamlit_baseweb-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4113 2023-07-06 00:11:51.143581 streamlit_baseweb-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2190 2023-07-05 22:27:03.000000 streamlit_baseweb-0.1.0/README.md
--rw-rw-rw-   0        0        0      911 2023-07-06 00:07:22.000000 streamlit_baseweb-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 00:11:51.144582 streamlit_baseweb-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-05 23:57:38.000000 streamlit_baseweb-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.030547 streamlit_baseweb-0.1.0/streamlit_baseweb/
--rw-rw-rw-   0        0        0     4453 2023-07-06 00:04:10.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.005701 streamlit_baseweb-0.1.0/streamlit_baseweb/button/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.059687 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/
--rw-rw-rw-   0        0        0      859 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/asset-manifest.json
--rw-rw-rw-   0        0        0     1870 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/index.html
--rw-rw-rw-   0        0        0      564 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js
--rw-rw-rw-   0        0        0     1183 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.007468 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.095958 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/
--rw-rw-rw-   0        0        0   655678 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js
--rw-rw-rw-   0        0        0     1803 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1790536 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map
--rw-rw-rw-   0        0        0     1191 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js
--rw-rw-rw-   0        0        0     3410 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map
--rw-rw-rw-   0        0        0     1590 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js
--rw-rw-rw-   0        0        0     8309 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.009093 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.107736 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/
--rw-rw-rw-   0        0        0      859 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/asset-manifest.json
--rw-rw-rw-   0        0        0     1870 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/index.html
--rw-rw-rw-   0        0        0      564 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js
--rw-rw-rw-   0        0        0     1183 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.010532 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.140583 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/
--rw-rw-rw-   0        0        0   700106 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js
--rw-rw-rw-   0        0        0     1803 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1996642 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map
--rw-rw-rw-   0        0        0     1488 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js
--rw-rw-rw-   0        0        0     4819 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map
--rw-rw-rw-   0        0        0     1590 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js
--rw-rw-rw-   0        0        0     8309 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map
-drwxrwxrwx   0        0        0        0 2023-07-06 00:11:51.046114 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/
--rw-rw-rw-   0        0        0     4113 2023-07-06 00:11:50.000000 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1708 2023-07-06 00:11:50.000000 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 00:11:50.000000 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-06 00:11:50.000000 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-06 00:11:50.000000 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-06 00:11:50.000000 streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.983423 streamlit_baseweb-0.1.1/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-07-06 00:06:11.000000 streamlit_baseweb-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4755 2023-07-06 00:17:08.982449 streamlit_baseweb-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2832 2023-07-06 00:14:27.000000 streamlit_baseweb-0.1.1/README.md
+-rw-rw-rw-   0        0        0      911 2023-07-06 00:16:01.000000 streamlit_baseweb-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 00:17:08.983423 streamlit_baseweb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-06 00:16:01.000000 streamlit_baseweb-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.913210 streamlit_baseweb-0.1.1/streamlit_baseweb/
+-rw-rw-rw-   0        0        0     4453 2023-07-06 00:04:10.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.890997 streamlit_baseweb-0.1.1/streamlit_baseweb/button/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.930452 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/
+-rw-rw-rw-   0        0        0      859 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1870 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/index.html
+-rw-rw-rw-   0        0        0      564 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js
+-rw-rw-rw-   0        0        0     1183 2023-07-06 00:07:45.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.891995 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.951924 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/
+-rw-rw-rw-   0        0        0   655678 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1790536 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map
+-rw-rw-rw-   0        0        0     1191 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js
+-rw-rw-rw-   0        0        0     3410 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map
+-rw-rw-rw-   0        0        0     1590 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js
+-rw-rw-rw-   0        0        0     8309 2023-07-06 00:07:46.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.893017 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.958908 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/
+-rw-rw-rw-   0        0        0      859 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1870 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/index.html
+-rw-rw-rw-   0        0        0      564 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js
+-rw-rw-rw-   0        0        0     1183 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.893998 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.981071 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/
+-rw-rw-rw-   0        0        0   700106 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1996642 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map
+-rw-rw-rw-   0        0        0     1488 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js
+-rw-rw-rw-   0        0        0     4819 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map
+-rw-rw-rw-   0        0        0     1590 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js
+-rw-rw-rw-   0        0        0     8309 2023-07-03 16:11:57.000000 streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map
+drwxrwxrwx   0        0        0        0 2023-07-06 00:17:08.924095 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/
+-rw-rw-rw-   0        0        0     4755 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1708 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-06 00:17:08.000000 streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/top_level.txt
```

### Comparing `streamlit_baseweb-0.1.0/LICENSE` & `streamlit_baseweb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/PKG-INFO` & `streamlit_baseweb-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_baseweb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,19 +47,30 @@
 
 ## Usage
 
 To use the Baseweb components in your Streamlit application, you need to import the necessary components from the '**streamlit_baseweb**' module and utilize them in your code. Here's an example:
 
 ```python
 import streamlit as st
-from streamlit_baseweb import base_web_modal
+from streamlit_baseweb import base_web_modal, base_web_button
 
 st.title("Testing Streamlit Baseweb")
-if st.button(label="open modal"):
-    base_web_modal(title="modal", body="testing modal", key="base_web_modal")
+if base_web_button(size="large", shape="pill", kind="secondary"):
+    base_web_modal(
+        title="This is a test modal",
+        body="""
+                Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium 
+                doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae 
+                vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, 
+                sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est,
+    """,
+        key="modal",
+    )
+if st.session_state.get("modal"):
+    st.success("Confirmation received from modal")
 
 ```
 
 For more details on available components and their usage, refer to the package documentation.
 
 ## Roadmap
 Elements will be integrated as per the below priority ranking:
```

### Comparing `streamlit_baseweb-0.1.0/README.md` & `streamlit_baseweb-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,19 +12,30 @@
 
 ## Usage
 
 To use the Baseweb components in your Streamlit application, you need to import the necessary components from the '**streamlit_baseweb**' module and utilize them in your code. Here's an example:
 
 ```python
 import streamlit as st
-from streamlit_baseweb import base_web_modal
+from streamlit_baseweb import base_web_modal, base_web_button
 
 st.title("Testing Streamlit Baseweb")
-if st.button(label="open modal"):
-    base_web_modal(title="modal", body="testing modal", key="base_web_modal")
+if base_web_button(size="large", shape="pill", kind="secondary"):
+    base_web_modal(
+        title="This is a test modal",
+        body="""
+                Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium 
+                doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae 
+                vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, 
+                sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est,
+    """,
+        key="modal",
+    )
+if st.session_state.get("modal"):
+    st.success("Confirmation received from modal")
 
 ```
 
 For more details on available components and their usage, refer to the package documentation.
 
 ## Roadmap
 Elements will be integrated as per the below priority ranking:
```

### Comparing `streamlit_baseweb-0.1.0/pyproject.toml` & `streamlit_baseweb-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_baseweb"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Streamlit implementation of the Base Web library."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `streamlit_baseweb-0.1.0/setup.py` & `streamlit_baseweb-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_baseweb",
-    version="0.1.0",
+    version="0.1.1",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the Base Web library.",
     long_description="https://baseweb.design/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/baseweb_components",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/__init__.py` & `streamlit_baseweb-0.1.1/streamlit_baseweb/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/asset-manifest.json` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/index.html` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/precache-manifest.b5d74bd96e379274fd2ea14bfa52007c.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/service-worker.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/2.c1418e57.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/main.a61d4437.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map` & `streamlit_baseweb-0.1.1/streamlit_baseweb/button/build/static/js/runtime-main.6f7b4229.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/asset-manifest.json` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/index.html` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/precache-manifest.335beef11633fc996a1434855591b164.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/service-worker.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/2.5aa23a28.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/main.fcdf4979.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map` & `streamlit_baseweb-0.1.1/streamlit_baseweb/modal/build/static/js/runtime-main.6f7b4229.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/PKG-INFO` & `streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-baseweb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,19 +47,30 @@
 
 ## Usage
 
 To use the Baseweb components in your Streamlit application, you need to import the necessary components from the '**streamlit_baseweb**' module and utilize them in your code. Here's an example:
 
 ```python
 import streamlit as st
-from streamlit_baseweb import base_web_modal
+from streamlit_baseweb import base_web_modal, base_web_button
 
 st.title("Testing Streamlit Baseweb")
-if st.button(label="open modal"):
-    base_web_modal(title="modal", body="testing modal", key="base_web_modal")
+if base_web_button(size="large", shape="pill", kind="secondary"):
+    base_web_modal(
+        title="This is a test modal",
+        body="""
+                Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium 
+                doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae 
+                vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, 
+                sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est,
+    """,
+        key="modal",
+    )
+if st.session_state.get("modal"):
+    st.success("Confirmation received from modal")
 
 ```
 
 For more details on available components and their usage, refer to the package documentation.
 
 ## Roadmap
 Elements will be integrated as per the below priority ranking:
```

### Comparing `streamlit_baseweb-0.1.0/streamlit_baseweb.egg-info/SOURCES.txt` & `streamlit_baseweb-0.1.1/streamlit_baseweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

