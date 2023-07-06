# Comparing `tmp/omneer-0.12.tar.gz` & `tmp/omneer-0.13-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omneer-0.12.tar", last modified: Sat Jul  1 07:13:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

