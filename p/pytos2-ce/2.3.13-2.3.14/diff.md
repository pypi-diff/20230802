# Comparing `tmp/pytos2-ce-2.3.13.tar.gz` & `tmp/pytos2_ce-2.3.14-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytos2-ce-2.3.13.tar", last modified: Thu May  4 13:08:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

