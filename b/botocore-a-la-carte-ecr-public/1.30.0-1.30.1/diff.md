# Comparing `tmp/botocore-a-la-carte-ecr-public-1.30.0.tar.gz` & `tmp/botocore_a_la_carte_ecr_public-1.30.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ecr-public-1.30.0.tar", last modified: Tue Jul  4 01:44:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

