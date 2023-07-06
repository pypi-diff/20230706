# Comparing `tmp/pyautotrace-0.0.2.tar.gz` & `tmp/pyautotrace-0.0.3-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyautotrace-0.0.2.tar", last modified: Mon Oct  3 03:15:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

