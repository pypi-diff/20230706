# Comparing `tmp/brick-james-0.2.1.tar.gz` & `tmp/brick_james-0.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/odell/brick/dist/tmp8qkv04fu/brick-james-0.2.1.tar", last modified: Tue Nov 22 22:55:31 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

