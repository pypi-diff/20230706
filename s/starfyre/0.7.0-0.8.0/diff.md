# Comparing `tmp/starfyre-0.7.0.tar.gz` & `tmp/starfyre-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.7.0.tar", max compression
+gzip compressed data, was "starfyre-0.8.0.tar", max compression
```

## Comparing `starfyre-0.7.0.tar` & `starfyre-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4382 2023-07-05 07:48:48.829507 starfyre-0.7.0/README.md
--rw-r--r--   0        0        0      454 2023-07-05 07:48:48.829507 starfyre-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      949 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/__main__.py
--rw-r--r--   0        0        0     4539 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/component.py
--rw-r--r--   0        0        0     3550 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-07-05 07:48:48.829507 starfyre-0.7.0/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/js/store.js
--rw-r--r--   0        0        0     9071 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-07-05 07:48:48.833507 starfyre-0.7.0/starfyre/transpiler.py
--rw-r--r--   0        0        0     4920 1970-01-01 00:00:00.000000 starfyre-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4751 2023-07-06 20:03:56.649057 starfyre-0.8.0/README.md
+-rw-r--r--   0        0        0      454 2023-07-06 20:03:56.649057 starfyre-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      949 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/__main__.py
+-rw-r--r--   0        0        0     5392 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/component.py
+-rw-r--r--   0        0        0     3550 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/js/store.js
+-rw-r--r--   0        0        0     9071 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/transpiler.py
+-rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 starfyre-0.8.0/PKG-INFO
```

### Comparing `starfyre-0.7.0/README.md` & `starfyre-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -90,25 +90,33 @@
 If you're feeling curious. You can take a look at a more detailed architecture here.
 
 If you still need help to get started, feel free to reach out on our community discord.
 
 
 ## ⚙️  Developing Locally
 
-1. Install the dependencies `poetry install`
-2. Run the script `./build.sh`. This command will run the build process in starfyre against the test application in `test-application` directory.
+Python version 3.10
+
+1. Fork this [repo](https://github.com/sparckles/starfyre)
+2. Clone this repo - `git clone https://github.com/sparckles/starfyre`
+3. Go in to the starfire directory - `cd starfyre`
+4. Download poetry `curl -sSL https://install.python-poetry.org/ | python3 -`
+5. Install the dependencies `poetry install`
+6. Activate poetry virtual enviromente `poetry shell`
+7. Run the script `./build.sh`. This command will run the build process in starfyre against the test application in `test-application` directory.
   - The `build.sh` file is a simple script that runs two commands sequentially.
     - `python -m starfyre --dev=True --path="test-application/"`
     - `python -m starfyre --build=True --path="test-application/"`
         - The `path` variable here is the path to our application.
         - The `dev` flag here is used to start the compilation and create the `build` directory. 
         - The `build` directory is basically a python package that contains all the compiled files. We use the `--build` flag to run that package.
 
-3. You can find a small test application in the `test-application` directory.
-4. Navigate to `test-application/dist` and open `index.html` in your browser to see the output.
+8. You can find a small test application in the `test-application` directory.
+9. Navigate to `cd test-application/dist`.
+10. Open `index.html` in your browser to see the output, run `explorer.exe index.html`.
 
 ## Running the sample app with Docker
 
 #### Ideally, we should not be needing this. But if you are having trouble running the sample app locally, you can try this.
 
 1. Build the image `docker build --tag starfyre .`
 2. Run the container `docker run -v ./test-application:/app/test-application/ starfyre`
```

### Comparing `starfyre-0.7.0/starfyre/__init__.py` & `starfyre-0.8.0/starfyre/__init__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/starfyre/__main__.py` & `starfyre-0.8.0/starfyre/__main__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/starfyre/compiler.py` & `starfyre-0.8.0/starfyre/compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 import os
+import re
 from pathlib import Path
 
 
 def get_fyre_files(project_dir):
     fyre_files = []
     for file in os.listdir(project_dir):
         if file.endswith(".fyre"):
             fyre_files.append(file)
     return fyre_files
 
+def resolve_css_import(css_file_path: Path):
+    """Read a css file and save it's content to a list"""
+    css_content = [] 
 
-def parse(fyre_file_name):
+    with open(css_file_path.resolve(), "r") as import_file:
+        for line in import_file.readlines():
+            css_content.append(line)
+
+    return css_content           
+
+
+def parse(fyre_file_name): 
     def remove_empty_lines_from_end(lines):
         while lines and lines[-1] == "\n":
             lines.pop()
 
         while lines and lines[0] == "\n":
             lines.pop(0)
 
@@ -25,28 +36,37 @@
     current_line_type = "python"
     python_lines = []
     css_lines = []
     pyml_lines = []
     js_lines = []
     client_side_python = []
 
+    # regex pattern to match if a line is a css import, e.g. import "style.css"
+    css_import_pattern = re.compile(r"^import\s[\"\'](.*?\.css)[\"\']")
+    
     with open(fyre_file_name, "r") as fyre_file:
         for line in fyre_file.readlines():
+            css_import_match = css_import_pattern.search(line)
             if line.startswith("<style"):
                 current_line_type = "css"
                 continue
             elif line.startswith("<pyml"):
                 current_line_type = "pyml"
                 continue
             elif line.startswith("<script"):
                 current_line_type = "js"
                 continue
             elif line.startswith("--client"):
                 current_line_type = "client"  # this is a hack
                 continue
+            elif css_import_match:
+                css_import = css_import_match.group(1)
+                css_content = resolve_css_import(Path(css_import))
+                css_lines += css_content
+                continue
             elif (
                 "</style>" in line
                 or "</pyml>" in line
                 or "</script>" in line
                 or "--" in line
             ):
                 current_line_type = "python"
@@ -142,19 +162,19 @@
 
     main_content = python_transpiled_string(
         pyml_lines, css_lines, js_lines, client_side_python, output_file_name
     )
 
     final_python_lines.append(main_content)
 
-    file_name = output_file_name.split("/")[-1]
+    file_name = output_file_name.split("/")[-1]                 #getting the file itself "without the path"
     output_file_name = project_dir / "build" / file_name
 
     with open(output_file_name, "w") as output_file:
-        output_file.write("".join(final_python_lines))
+        output_file.write("".join(final_python_lines))          #result of the transpiled
 
 
 def compile(entry_file_name):
     project_dir = Path(os.path.dirname(entry_file_name))
 
     build_dir = project_dir / "build"
     build_dir.mkdir(exist_ok=True)
```

### Comparing `starfyre-0.7.0/starfyre/component.py` & `starfyre-0.8.0/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/starfyre/dom_methods.py` & `starfyre-0.8.0/starfyre/dom_methods.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/starfyre/js/store.js` & `starfyre-0.8.0/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/starfyre/parser.py` & `starfyre-0.8.0/starfyre/parser.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/starfyre/transpiler.py` & `starfyre-0.8.0/starfyre/transpiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.7.0/PKG-INFO` & `starfyre-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfyre
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python Framework for writing Reactive web Front-Ends
 License: BSD 2.0
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -106,25 +106,33 @@
 If you're feeling curious. You can take a look at a more detailed architecture here.
 
 If you still need help to get started, feel free to reach out on our community discord.
 
 
 ## ⚙️  Developing Locally
 
-1. Install the dependencies `poetry install`
-2. Run the script `./build.sh`. This command will run the build process in starfyre against the test application in `test-application` directory.
+Python version 3.10
+
+1. Fork this [repo](https://github.com/sparckles/starfyre)
+2. Clone this repo - `git clone https://github.com/sparckles/starfyre`
+3. Go in to the starfire directory - `cd starfyre`
+4. Download poetry `curl -sSL https://install.python-poetry.org/ | python3 -`
+5. Install the dependencies `poetry install`
+6. Activate poetry virtual enviromente `poetry shell`
+7. Run the script `./build.sh`. This command will run the build process in starfyre against the test application in `test-application` directory.
   - The `build.sh` file is a simple script that runs two commands sequentially.
     - `python -m starfyre --dev=True --path="test-application/"`
     - `python -m starfyre --build=True --path="test-application/"`
         - The `path` variable here is the path to our application.
         - The `dev` flag here is used to start the compilation and create the `build` directory. 
         - The `build` directory is basically a python package that contains all the compiled files. We use the `--build` flag to run that package.
 
-3. You can find a small test application in the `test-application` directory.
-4. Navigate to `test-application/dist` and open `index.html` in your browser to see the output.
+8. You can find a small test application in the `test-application` directory.
+9. Navigate to `cd test-application/dist`.
+10. Open `index.html` in your browser to see the output, run `explorer.exe index.html`.
 
 ## Running the sample app with Docker
 
 #### Ideally, we should not be needing this. But if you are having trouble running the sample app locally, you can try this.
 
 1. Build the image `docker build --tag starfyre .`
 2. Run the container `docker run -v ./test-application:/app/test-application/ starfyre`
```

