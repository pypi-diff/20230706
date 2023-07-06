# Comparing `tmp/invisible-watermark-0.1.5.tar.gz` & `tmp/invisible_watermark-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invisible-watermark-0.1.5.tar", last modified: Mon Feb  1 04:00:15 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

