# Comparing `tmp/dithering-0.1.18.tar.gz` & `tmp/dithering-0.1.19-pp310-pypy310_pp73-manylinux_2_5_i686.manylinux1_i686.whl.zip`

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

