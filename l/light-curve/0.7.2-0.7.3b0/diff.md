# Comparing `tmp/light_curve-0.7.2.tar.gz` & `tmp/light_curve-0.7.3b0-pp38-pypy38_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

