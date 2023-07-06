# Comparing `tmp/cPyparsing-2.4.7.2.0.0.tar.gz` & `tmp/cPyparsing-2.4.7.2.1.0-cp37-cp37m-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cPyparsing-2.4.7.2.0.0.tar", last modified: Wed Jul  5 04:05:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

