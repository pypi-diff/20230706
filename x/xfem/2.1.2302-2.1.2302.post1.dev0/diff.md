# Comparing `tmp/xfem-2.1.2302.tar.gz` & `tmp/xfem-2.1.2302.post1.dev0-cp39-cp39-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfem-2.1.2302.tar", last modified: Wed Jul  5 21:59:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

