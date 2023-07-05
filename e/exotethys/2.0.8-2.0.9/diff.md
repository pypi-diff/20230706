# Comparing `tmp/exotethys-2.0.8.tar.gz` & `tmp/exotethys-2.0.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exotethys-2.0.8.tar", last modified: Mon Nov 28 17:23:24 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

