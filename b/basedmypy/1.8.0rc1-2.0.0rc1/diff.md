# Comparing `tmp/basedmypy-1.8.0rc1.tar.gz` & `tmp/basedmypy-2.0.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedmypy-1.8.0rc1.tar", last modified: Mon Apr 17 09:17:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

