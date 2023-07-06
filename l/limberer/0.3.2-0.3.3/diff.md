# Comparing `tmp/limberer-0.3.2.tar.gz` & `tmp/limberer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.3.2.tar", last modified: Wed Jul  5 21:44:04 2023, max compression
+gzip compressed data, was "limberer-0.3.3.tar", last modified: Thu Jul  6 07:10:10 2023, max compression
```

## Comparing `limberer-0.3.2.tar` & `limberer-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.3.2/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.3.2/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.3.2/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     9524 2023-07-05 21:44:04.253697 limberer-0.3.2/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     7462 2023-07-04 03:21:11.000000 limberer-0.3.2/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-05 19:36:49.000000 limberer-0.3.2/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-05 21:44:04.253697 limberer-0.3.2/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.249698 limberer-0.3.2/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    11884 2023-07-05 19:36:00.000000 limberer-0.3.2/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6752 2023-07-04 03:01:36.000000 limberer-0.3.2/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5535 2023-07-04 03:22:51.000000 limberer-0.3.2/src/limberer/static/assets/core.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.3.2/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.3.2/src/limberer/static/assets/style.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.3.2/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.3.2/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      363 2023-07-04 00:11:03.000000 limberer-0.3.2/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3887 2023-07-04 03:17:45.000000 limberer-0.3.2/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1643 2023-07-04 02:27:36.000000 limberer-0.3.2/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.3.2/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.3.2/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-04 01:55:47.000000 limberer-0.3.2/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      576 2023-07-05 19:36:31.000000 limberer-0.3.2/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-05 21:44:04.253697 limberer-0.3.2/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     9524 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-05 21:44:04.000000 limberer-0.3.2/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.3.3/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.3.3/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.3.3/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    10068 2023-07-06 07:10:10.142728 limberer-0.3.3/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     8006 2023-07-06 07:07:28.000000 limberer-0.3.3/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-06 07:09:47.000000 limberer-0.3.3/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-06 07:10:10.142728 limberer-0.3.3/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.138728 limberer-0.3.3/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    12673 2023-07-06 06:43:30.000000 limberer-0.3.3/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6752 2023-07-04 03:01:36.000000 limberer-0.3.3/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-06 07:09:08.000000 limberer-0.3.3/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.3.3/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.3.3/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.3.3/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.3.3/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      363 2023-07-04 00:11:03.000000 limberer-0.3.3/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3887 2023-07-04 03:17:45.000000 limberer-0.3.3/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1643 2023-07-04 02:27:36.000000 limberer-0.3.3/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.3.3/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.3.3/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      381 2023-07-06 06:48:22.000000 limberer-0.3.3/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.3.3/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:10:10.142728 limberer-0.3.3/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    10068 2023-07-06 07:10:10.000000 limberer-0.3.3/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-06 07:10:10.000000 limberer-0.3.3/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-06 07:10:10.000000 limberer-0.3.3/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-06 07:10:10.000000 limberer-0.3.3/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-06 07:10:10.000000 limberer-0.3.3/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-06 07:10:10.000000 limberer-0.3.3/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.3.2/LICENSE` & `limberer-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/PKG-INFO` & `limberer-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.3.2
+Version: 0.3.3
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -137,18 +137,33 @@
   { type = "toc" },
   { name = "example", type = "section", title = "Example" },
   { name = "example2", type = "section", title = "Example2", sectionoption = "value" },
   ...
 ]
 ```
 
-### Sections
+### Section Templates
 
-Sections are a mix of Markdown (and, in some cases, HTML), where most document
-content is written. A section can begin with a block of Markdown metadata:
+Out of the box, `limberer` comes with some initial section templates:
+
+* `cover`: A title page section.
+* `toc`: A table of contents section.
+* `section`: The underlying template for custom sections.
+
+Additionally, `limberer` supports the following template-like pseudo-sections:
+
+* `appendix_start`: Subsequent sections will be treated as appendices.
+* `appendix_end`: Disables the above setting; subsequent sections are not
+  treated as appendices. The appendix counter will not be cleared.
+
+### Custom Sections
+
+Custom sections ("sections") are a mix of Markdown (and, in some cases, HTML),
+where most document content is written. A section can begin with a block of
+Markdown metadata:
 
 ```markdown
 ---
 toc_header_level: 2
 columns: true
 title: Example3
 classes: foo bar baz
```

### Comparing `limberer-0.3.2/README.md` & `limberer-0.3.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -99,18 +99,33 @@
   { type = "toc" },
   { name = "example", type = "section", title = "Example" },
   { name = "example2", type = "section", title = "Example2", sectionoption = "value" },
   ...
 ]
 ```
 
-### Sections
+### Section Templates
 
-Sections are a mix of Markdown (and, in some cases, HTML), where most document
-content is written. A section can begin with a block of Markdown metadata:
+Out of the box, `limberer` comes with some initial section templates:
+
+* `cover`: A title page section.
+* `toc`: A table of contents section.
+* `section`: The underlying template for custom sections.
+
+Additionally, `limberer` supports the following template-like pseudo-sections:
+
+* `appendix_start`: Subsequent sections will be treated as appendices.
+* `appendix_end`: Disables the above setting; subsequent sections are not
+  treated as appendices. The appendix counter will not be cleared.
+
+### Custom Sections
+
+Custom sections ("sections") are a mix of Markdown (and, in some cases, HTML),
+where most document content is written. A section can begin with a block of
+Markdown metadata:
 
 ```markdown
 ---
 toc_header_level: 2
 columns: true
 title: Example3
 classes: foo bar baz
```

#### html2text {}

```diff
@@ -26,17 +26,24 @@
 will be rendered against the `template/section.html` template, but the template
 used can be changed via an `alt = "othertemplate"` section list setting. ###
 Project TOML ```toml title = "Example Document" subheading = "..."
 #globaloption=value #... authors = [ { name = "Example Person", email =
 "example@example.com" }, ... ] sections = [ { type = "cover" }, { type = "toc"
 }, { name = "example", type = "section", title = "Example" }, { name =
 "example2", type = "section", title = "Example2", sectionoption = "value" },
-... ] ``` ### Sections Sections are a mix of Markdown (and, in some cases,
-HTML), where most document content is written. A section can begin with a block
-of Markdown metadata: ```markdown --- toc_header_level: 2 columns: true title:
+... ] ``` ### Section Templates Out of the box, `limberer` comes with some
+initial section templates: * `cover`: A title page section. * `toc`: A table of
+contents section. * `section`: The underlying template for custom sections.
+Additionally, `limberer` supports the following template-like pseudo-sections:
+* `appendix_start`: Subsequent sections will be treated as appendices. *
+`appendix_end`: Disables the above setting; subsequent sections are not treated
+as appendices. The appendix counter will not be cleared. ### Custom Sections
+Custom sections ("sections") are a mix of Markdown (and, in some cases, HTML),
+where most document content is written. A section can begin with a block of
+Markdown metadata: ```markdown --- toc_header_level: 2 columns: true title:
 Example3 classes: foo bar baz --- ``` The metadata options are merged with the
 section entry options. Currently supported options are the following: *
 `toc_header_level`: Header level limit to use for table of contents entry
 generation. * `columns`: Whether or not to use the 2-column format for the
 section. * `title`: Section title for 2-column format. * `classes`: List of
 HTML class names to apply to the section (``) #### Tables Tables can be written
 using the pipe-delimited GitHub-flavored Markdown convention, or with HTML
```

### Comparing `limberer-0.3.2/pyproject.toml` & `limberer-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.3.2/src/limberer/__init__.py` & `limberer-0.3.3/src/limberer/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,17 +82,34 @@
     print(f"error: invalid path {repr(path)} references outside of project directory.")
     sys.exit(1)
   return open(path, mode)
 
 footnotecount = 1
 isheader = re.compile('h[1-9]')
 headercount = 0
+appendix = False
+appendix_count = 0
+
+alph = "AABCDEFGHIJKLMNOPQRSTUVWXYZ"
+def appendixify(n):
+  if n == 0:
+    return "A"
+  d = []
+  while n:
+    d.append((n % 26))
+    n //= 26
+  r = []
+  for _d in d[::-1]:
+    r.append(alph[_d])
+  r[-1] = chr(65+d[0])
+  return ''.join(r)
 
 def convert(path, opts, toc, args):
   global headercount
+  global appendix_count
   #print("convert(" + repr(path) + ")")
   proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
   if proc1.returncode != 0:
     sys.stderr.write("error running initial pandoc command: \n")
     sys.stderr.buffer.write(proc1.stderr)
     sys.stderr.write("\n")
     sys.exit(1)
@@ -115,22 +132,30 @@
   o2 = ow.read()
 
   if len(_headers) == 1:
     headers = _headers[0]
     headercount += len(headers)
 
   if "columns" in opts:
-    toc.append(opts | {"name": opts['section_name'] + "-columns-title", "issubsection": False})
+    ax = {}
+    if appendix:
+      ax['appendix_n'] = appendixify(appendix_count)
+      appendix_count += 1
+    toc.append(opts | {"name": opts['section_name'] + "-columns-title", "issubsection": False} | ax)
 
-  #print(repr(headers))
   header_level = int(opts.get('toc_header_level', ['1'])[0])
 
+  ah = False
   for h in headers:
+    ax = {}
+    if appendix and not ah and h.level == 1:
+      ax['appendix_n'] = appendixify(appendix_count)
+      ah = True
     if h.level <= header_level:
-      toc.append(opts | {"name": opts['section_name'] + "-" + h.identifier, "issubsection": h.level != 1})
+      toc.append(opts | {"name": opts['section_name'] + "-" + h.identifier, "issubsection": h.level != 1} | ax)
 
   # pass back to pandoc
   proc2 = subprocess.run(['pandoc', '-f', 'json',
                           '-t', 'html',
                           '--wrap=none'],
                          input=o2, text=True,
                          capture_output=True)
@@ -199,14 +224,16 @@
     else:
       print("project.toml not found in template path " + repr(args.template) + ".... using default.")
       shutil.copyfile(os.path.join(staticpath, "project.toml"),
                 os.path.join(absprojpath, projname + ".toml"))
 
 def build(args):
   global footnotecount
+  global appendix
+  global appendix_count
 
   config = args.config
   if not os.path.exists(config):
     sys.stderr.write(f"error: '{config}' not found.\n")
     sys.exit(1)
   if not os.path.isfile(config):
     sys.stderr.write(f"error: '{config}' is not a file.\n")
@@ -228,27 +255,24 @@
 
   sections = []
   toc = []
 
   for i in range(len(config['sections'])):
     section = config['sections'][i]
     if section['type'] == 'section':
-      # markdown
       section_name = section['name']
       section_path = 'sections/{}.md'.format(section['name'])
       content = open_subpath(section_path, 'rb').read()
-      #print(repr(content))
-      #content = content.decode('utf-8')
-      #md = markdown.Markdown(extensions=["meta"])
-      #html = md.convert(content)
-      #opts = md.Meta | section
       opts = {} | section
       opts['section_name'] = section_name
+      if appendix:
+        opts['appendix'] = True
       html = convert(section_path, opts, toc, args)
-      #print("opts: " + repr(opts))
+      if appendix:
+        appendix_count += 1
       footnotes = ""
       soup = BeautifulSoup(html, 'html.parser')
       _sns = soup.find_all(lambda e: e.name == 'section' and e.attrs.get('id')!=None)
       for _sn in _sns:
         _snc = [c for c in _sn.children if c != "\n"]
         if len(_snc) > 0:
           if re.match(isheader, _snc[0].name):
@@ -295,21 +319,32 @@
       if "alt" in section:
         template = open_subpath('templates/{}.html'.format(section['alt']), 'r').read()
       r = chevron.render(template, opts)
       sections.append(r)
     elif section['type'] == 'toc':
       # defer until after we get through everything else
       sections.append(section)
+    elif section['type'] == 'appendix_start':
+      appendix = True
+    elif section['type'] == 'appendix_end':
+      appendix = False
+    #elif section['type'] == 'appendix_reset':
+    #  appendix_count = 0
     else:
       # assume in templates/
       template = open_subpath('templates/{}.html'.format(section['type']), 'r').read()
       r = chevron.render(template, config)
       sections.append(r)
       if section['type'] != 'cover' and "title" in section:
-        toc.append(opts | {"name": section['type'], "issubsection": False})
+        name = section['type']
+        ax = {}
+        if appendix:
+          ax['appendix_n'] = appendixify(appendix_count)
+          appendix_count += 1
+        toc.append(opts | {"name": name, "issubsection": False} | ax)
 
   for section in sections:
     if type(section) == str:
       body += section
       body += "\n"
     else:
       if section['type'] == 'toc':
```

### Comparing `limberer-0.3.2/src/limberer/pf.py` & `limberer-0.3.3/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/assets/core.css` & `limberer-0.3.3/src/limberer/static/assets/core.css`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 html {
   color: black;
   font-family: Arial;
   font-size: 10pt;
   font-weight: 300;
   line-height: 1.0;
+  counter-reset: appendix;
 }
 
 strong {
   font-weight: bold;
 }
 
 body {
@@ -365,9 +366,11 @@
   color: inherit;
 }
 .footnote-back {
   text-decoration: none;
   color: inherit;
 }
 
-
-
+article.appendix>.article-body>h1:nth-of-type(1):before {
+  content: "Appendix " counter(appendix, upper-alpha) ": ";
+  counter-increment: appendix;
+}
```

### Comparing `limberer-0.3.2/src/limberer/static/assets/logo.svg` & `limberer-0.3.3/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/assets/style.css` & `limberer-0.3.3/src/limberer/static/assets/style.css`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/images/test1.jpg` & `limberer-0.3.3/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/sections/example.md` & `limberer-0.3.3/src/limberer/static/sections/example.md`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/sections/example2.md` & `limberer-0.3.3/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/templates/cover.html` & `limberer-0.3.3/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.3.2/src/limberer/static/templates/toc.html` & `limberer-0.3.3/src/limberer/static/templates/toc.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
     <article id="contents">
       <h3>Table of Contents</h3>
       <ul class="toc">
       {{#sections}}
       {{^issubsection}}
-        <li><a class="toc" href="#{{name}}"><div href="#{{name}}" class="toctext"></div><div href="#{{name}}" class="tocpagenr"></div></a></li>
+        <li><a class="toc" href="#{{name}}">{{#appendix_n}}Appendix {{.}}:&nbsp;{{/appendix_n}}<div href="#{{name}}" class="toctext"></div><div href="#{{name}}" class="tocpagenr"></div></a></li>
       {{/issubsection}}
       {{#issubsection}}
         <ul class="toc">
-          <li><a class="toc" href="#{{name}}"><div href="#{{name}}" class="toctext"></div><div href="#{{name}}" class="tocpagenr"></div></a></li>
+          <li><a class="toc" href="#{{name}}">{{#appendix_n}}Appendix {{.}}:&nbsp;{{/appendix_n}}<div href="#{{name}}" class="toctext"></div><div href="#{{name}}" class="tocpagenr"></div></a></li>
         </ul>
       {{/issubsection}}
       {{/sections}}
       </ul>
     </article>
```

### Comparing `limberer-0.3.2/src/limberer.egg-info/PKG-INFO` & `limberer-0.3.3/src/limberer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.3.2
+Version: 0.3.3
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -137,18 +137,33 @@
   { type = "toc" },
   { name = "example", type = "section", title = "Example" },
   { name = "example2", type = "section", title = "Example2", sectionoption = "value" },
   ...
 ]
 ```
 
-### Sections
+### Section Templates
 
-Sections are a mix of Markdown (and, in some cases, HTML), where most document
-content is written. A section can begin with a block of Markdown metadata:
+Out of the box, `limberer` comes with some initial section templates:
+
+* `cover`: A title page section.
+* `toc`: A table of contents section.
+* `section`: The underlying template for custom sections.
+
+Additionally, `limberer` supports the following template-like pseudo-sections:
+
+* `appendix_start`: Subsequent sections will be treated as appendices.
+* `appendix_end`: Disables the above setting; subsequent sections are not
+  treated as appendices. The appendix counter will not be cleared.
+
+### Custom Sections
+
+Custom sections ("sections") are a mix of Markdown (and, in some cases, HTML),
+where most document content is written. A section can begin with a block of
+Markdown metadata:
 
 ```markdown
 ---
 toc_header_level: 2
 columns: true
 title: Example3
 classes: foo bar baz
```

### Comparing `limberer-0.3.2/src/limberer.egg-info/SOURCES.txt` & `limberer-0.3.3/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

