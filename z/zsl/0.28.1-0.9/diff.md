# Comparing `tmp/zsl-0.28.1.tar.gz` & `tmp/zsl-0.9-py2-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsl-0.28.1.tar", last modified: Wed Aug  2 10:37:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

