# Comparing `tmp/pycsgogpt-0.1.2.tar.gz` & `tmp/pycsgogpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsgogpt-0.1.2.tar", max compression
+gzip compressed data, was "pycsgogpt-0.1.3.tar", max compression
```

## Comparing `pycsgogpt-0.1.2.tar` & `pycsgogpt-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1024 2023-06-30 22:47:26.671280 pycsgogpt-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-30 22:47:26.671280 pycsgogpt-0.1.2/pycsgogpt/__init__.py
--rw-r--r--   0        0        0      667 2023-06-30 22:47:26.671280 pycsgogpt-0.1.2/pycsgogpt/__main__.py
--rw-r--r--   0        0        0     2218 2023-06-30 22:47:26.671280 pycsgogpt-0.1.2/pycsgogpt/csgo_chatbot.py
--rw-r--r--   0        0        0      807 2023-06-30 22:47:26.671280 pycsgogpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 pycsgogpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1024 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pycsgogpt/__init__.py
+-rw-r--r--   0        0        0      715 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pycsgogpt/__main__.py
+-rw-r--r--   0        0        0     2218 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pycsgogpt/csgo_chatbot.py
+-rw-r--r--   0        0        0      807 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 pycsgogpt-0.1.3/PKG-INFO
```

### Comparing `pycsgogpt-0.1.2/README.md` & `pycsgogpt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.2/pycsgogpt/__main__.py` & `pycsgogpt-0.1.3/pycsgogpt/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,7 +15,11 @@
         print(f"Connection refused. Make sure you add `-netconport {telnet_port}` to the CSGO server launch options.")
     except ConnectionAbortedError:
         print("Bye!")
 
 def main():
     app.command()(entry)
     app()
+    
+    
+if __name__ == "__main__":
+    main()
```

### Comparing `pycsgogpt-0.1.2/pycsgogpt/csgo_chatbot.py` & `pycsgogpt-0.1.3/pycsgogpt/csgo_chatbot.py`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.2/pyproject.toml` & `pycsgogpt-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "pycsgogpt"
-version = "0.1.2"
+version = "0.1.3"
 description = "CSGO Chatbot using OpenAI GPT-3.5 Turbo."
 authors = ["Aviv <4440524+nikeix@users.noreply.github.com>"]
 license = "MIT"
 keywords = ["csgo", "chatbot", "openai", "gpt"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `pycsgogpt-0.1.2/PKG-INFO` & `pycsgogpt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycsgogpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: CSGO Chatbot using OpenAI GPT-3.5 Turbo.
 Home-page: https://github.com/nikeix/pycsgogpt
 License: MIT
 Keywords: csgo,chatbot,openai,gpt
 Author: Aviv
 Author-email: 4440524+nikeix@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
```

