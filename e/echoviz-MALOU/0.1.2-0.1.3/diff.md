# Comparing `tmp/echoviz-MALOU-0.1.2.tar.gz` & `tmp/echoviz_MALOU-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoviz-MALOU-0.1.2.tar", last modified: Mon Apr  3 15:56:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

