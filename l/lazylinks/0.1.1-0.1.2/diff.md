# Comparing `tmp/lazylinks-0.1.1.tar.gz` & `tmp/lazylinks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazylinks-0.1.1.tar", last modified: Wed Jul  5 01:57:29 2023, max compression
+gzip compressed data, was "lazylinks-0.1.2.tar", last modified: Thu Jul  6 17:44:21 2023, max compression
```

## Comparing `lazylinks-0.1.1.tar` & `lazylinks-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-05 01:57:18.000000 lazylinks-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-05 01:57:18.000000 lazylinks-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 01:57:18.000000 lazylinks-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-05 01:57:29.340338 lazylinks-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-05 01:57:18.000000 lazylinks-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/lazylinks/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/lazylinks.mako
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/lazylinks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/lazylinks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-05 01:57:18.000000 lazylinks-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:57:29.340338 lazylinks-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:44:21.301756 lazylinks-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:44:21.297757 lazylinks-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:44:21.297757 lazylinks-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 17:44:11.000000 lazylinks-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-06 17:44:11.000000 lazylinks-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 17:44:11.000000 lazylinks-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-06 17:44:21.297757 lazylinks-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-06 17:44:11.000000 lazylinks-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:44:21.297757 lazylinks-0.1.2/lazylinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 17:44:11.000000 lazylinks-0.1.2/lazylinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-06 17:44:11.000000 lazylinks-0.1.2/lazylinks/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-06 17:44:11.000000 lazylinks-0.1.2/lazylinks/lazylinks.mako
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-06 17:44:11.000000 lazylinks-0.1.2/lazylinks/lazylinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 17:44:11.000000 lazylinks-0.1.2/lazylinks/wrap.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:44:21.297757 lazylinks-0.1.2/lazylinks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-06 17:44:21.000000 lazylinks-0.1.2/lazylinks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-06 17:44:21.000000 lazylinks-0.1.2/lazylinks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:44:21.000000 lazylinks-0.1.2/lazylinks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 17:44:21.000000 lazylinks-0.1.2/lazylinks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 17:44:21.000000 lazylinks-0.1.2/lazylinks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 17:44:21.000000 lazylinks-0.1.2/lazylinks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 17:44:11.000000 lazylinks-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:44:21.301756 lazylinks-0.1.2/setup.cfg
```

### Comparing `lazylinks-0.1.1/.github/workflows/python-publish.yml` & `lazylinks-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.1/.gitignore` & `lazylinks-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.1/LICENSE` & `lazylinks-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.1/PKG-INFO` & `lazylinks-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylinks
-Version: 0.1.1
+Version: 0.1.2
 Summary: Linktree-style links for lazy people
 Author-email: Samuel Colburn <samuel.colburn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Samuel Colburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lazylinks-0.1.1/README.md` & `lazylinks-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.1/lazylinks/dotdict.py` & `lazylinks-0.1.2/lazylinks/dotdict.py`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.1/lazylinks/lazylinks.mako` & `lazylinks-0.1.2/lazylinks/lazylinks.mako`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     <div class="links">
       % for link in section.links:
         % if 'href' in link and 'copy' in link:
           <a class="link"
           % if 'more' in link:
           ${link.more}
           % endif
-          href="${link.href}" target="_blank">
+          href="${link.href if 'wrap' not in link else link.wrap+'.html'}" target="_blank">
             <div class="tooltip hidden min">
               <i class="fa-solid fa-copy"></i>
             </div>
             <div class="inline-block">
               <i class="${link.icon}"></i> ${link.text}
               % if 'info' in link:
               <div class="info">${link.info}</div>
@@ -84,15 +84,15 @@
             </div>
           </a>
         % elif 'href' in link:
         <a class="link"
         % if 'more' in link:
         ${link.more}
         % endif
-        href="${link.href}" target="_blank">
+        href="${link.href if 'wrap' not in link else link.wrap+'.html'}" target="_blank">
           <i class="${link.icon}"></i> ${link.text}
           % if 'info' in link:
           <div class="info">${link.info}</div>
           % endif
         </a>
         % elif 'copy' in link:
         <div class="tooltip block">
```

#### html2text {}

```diff
@@ -9,22 +9,24 @@
 % if 'pronouns' in config:
 ${config.pronouns}
 % endif
 ${config.description}
 % for section in links:
 ${section.title}
 % for link in section.links: % if 'href' in link and 'copy' in link:
- if 'more' in link: ${link.more} % endif href="${link.href}" target="_blank">
+ if 'more' in link: ${link.more} % endif href="${link.href if 'wrap' not in
+link else link.wrap+'.html'}" target="_blank">
  ${link.text} % if 'info' in link:
 ${link.info}
 % endif
  Copy to clipboard
  % elif 'href' in link:
- if 'more' in link: ${link.more} % endif href="${link.href}" target="_blank">
-${link.text} % if 'info' in link:
+ if 'more' in link: ${link.more} % endif href="${link.href if 'wrap' not in
+link else link.wrap+'.html'}" target="_blank">  ${link.text} % if 'info' in
+link:
 ${link.info}
 % endif
  % elif 'copy' in link:
 Copy_to_clipboard__${link.text}
 % endif % endfor
 % endfor  % if 'qrcode' in config:
 [${config.qrcode}]
```

### Comparing `lazylinks-0.1.1/lazylinks/lazylinks.py` & `lazylinks-0.1.2/lazylinks/lazylinks.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,25 @@
     args = parser.parse_args()
 
     raw_data = yaml.safe_load(open(args.filename).read())
     raw_data["metadata"] = {"last_updated": datetime.now()}
     data = dotdict(raw_data)
 
     template = Template(filename=args.template)
+    wrap_template = Template(filename=os.path.join(dir_path, "wrap.mako"))
 
     if os.path.exists(args.static):
         shutil.copytree(args.static, "output", dirs_exist_ok=True)
     with open(os.path.join(args.output, "index.html"), "w") as outfile:
         outfile.write(template.render(**data))
-
+    for section in data.links:
+        for link in section.links:
+            if "wrap" in link:
+                with open(os.path.join(args.output, f"{link.wrap}.html"), "w") as wrap_outfile:
+                    wrap_data = {
+                        "config": data["config"],
+                        "link": link,
+                    }
+                    wrap_outfile.write(wrap_template.render(**wrap_data))
+        
 if __name__ == "__main__":
     main()
```

### Comparing `lazylinks-0.1.1/lazylinks.egg-info/PKG-INFO` & `lazylinks-0.1.2/lazylinks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylinks
-Version: 0.1.1
+Version: 0.1.2
 Summary: Linktree-style links for lazy people
 Author-email: Samuel Colburn <samuel.colburn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Samuel Colburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lazylinks-0.1.1/pyproject.toml` & `lazylinks-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lazylinks"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Samuel Colburn", email = "samuel.colburn@gmail.com"},
 ]
 description = "Linktree-style links for lazy people"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

