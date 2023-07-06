# Comparing `tmp/mypy-boto3-cloudcontrol-1.27.0.tar.gz` & `tmp/mypy_boto3_cloudcontrol-1.28.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudcontrol-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

