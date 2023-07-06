# Comparing `tmp/LNPLab-0.0.1.tar.gz` & `tmp/LNPLab-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LNPLab-0.0.1.tar", last modified: Thu Jun 22 06:51:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

