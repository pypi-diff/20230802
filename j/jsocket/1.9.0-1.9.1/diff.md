# Comparing `tmp/jsocket-1.9.0.tar.gz` & `tmp/jsocket-1.9.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsocket-1.9.0.tar", last modified: Tue Jan  3 21:32:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

