# Comparing `tmp/REMclust-1.0.tar.gz` & `tmp/REMclust-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REMclust-1.0.tar", last modified: Sun Apr 16 10:27:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

